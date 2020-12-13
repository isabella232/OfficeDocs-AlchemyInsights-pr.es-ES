---
title: Dispositivo en estado pendiente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652245"
---
# <a name="device-in-pending-state"></a>Dispositivo en estado pendiente

**Requisitos previos**

1. Si está configurando registros de dispositivos por primera vez, asegúrese de que ha revisado la [Introducción a la administración de dispositivos en Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , que le guiarán en la obtención de dispositivos bajo el control de Azure ad.
2. Si registra los dispositivos directamente en Azure AD y los inscribe en Intune, deberá asegurarse de que ha [configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) y de que el [otorgamiento de licencias](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) se realice primero.
3. Asegúrese de que tiene autorización para realizar operaciones en Azure AD y AD local. Solo un administrador global de Azure AD puede administrar la configuración de los registros de dispositivos. Además, si está configurando los registros automáticos en su Active Directory local, tendrá que ser administrador de Active Directory y AD FS (si procede).

El proceso de registro de Unión híbrida de Azure AD requiere que los dispositivos estén en la red corporativa. También funciona con VPN, pero hay algunas advertencias. Hemos oído que los clientes necesitan asistencia para solucionar el proceso de registro de Unión híbrida de Azure AD en circunstancias laborales remotas.

**Entorno de autenticación en la nube (mediante la sincronización de hash de contraseña de Azure AD o la autenticación de paso a través)**

Este flujo de registro también se conoce como "sincronización de sincronización".

Este es un desglose de lo que sucede durante el proceso de registro:

1. Windows 10 detecta el registro de punto de conexión de servicio (SCP) cuando el usuario inicia sesión en el dispositivo.

    1. En primer lugar, el dispositivo intenta recuperar información de inquilinos del SCP del lado cliente en el registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obtener más información, consulte [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Si se produce un error, el dispositivo se comunica con Active Directory local para obtener la información de inquilino de SCP. Para comprobar el SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Le recomendamos que habilite el SCP en Active Directory y solo use el SCP del lado cliente para la validación inicial.

2. Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD.

    Puede comprobar si el dispositivo puede tener acceso a los recursos de Microsoft en la cuenta del sistema mediante el [script de conectividad de registro de dispositivos de prueba](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en Active Directory local. Esto requiere línea de vista a controlador de dominio.

4. El objeto de dispositivo que tiene el certificado se sincroniza con Azure AD a través de Azure AD Connect. El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Connect. Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. En esta fase, debería poder ver el dispositivo de asunto en el estado "**pendiente**" en la hoja de dispositivos de Azure portal.

6. El registro se completará en el siguiente inicio de sesión de usuario en Windows 10.

    > [!NOTE]
    > Si está en VPN y cierre de sesión/inicio de sesión finaliza la Conectividad del dominio, puede desencadenar el registro manualmente. Para ello:
    >
    > Emita un `dsregcmd /join` mensaje local en el administrador o de forma remota a través de PSExec en su PC.
    >
    > Por ejemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para problemas comunes con el registro de dispositivos de Azure Active Directory, consulte [preguntas más frecuentes sobre dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).
