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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914020"
---
# <a name="device-in-pending-state"></a>Dispositivo en estado pendiente

**Requisitos previos:**

1. Si configura los registros de dispositivos por primera vez, asegúrese de que ha revisado Introducción a la administración de dispositivos en [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) que le guiará sobre cómo obtener dispositivos bajo el control de Azure AD.
2. Si vas a registrar dispositivos en Azure AD directamente e inscribirlos en Intune, deberás asegurarte de haber configurado [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) y tener las licencias [en](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) primer lugar.
3. Asegúrese de que está autorizado a realizar operaciones en Azure AD y AD local. Solo un administrador global de Azure AD puede administrar la configuración de registros de dispositivos. Además, si está configurando los registros automáticos en su Active Directory local, necesitará ser administrador de Active Directory y AD FS (si procede).

El proceso híbrido de registro de unión a Azure AD requiere que los dispositivos se den en la red corporativa. También funciona a través de VPN, pero hay algunas advertencias al respecto. Hemos escuchado a los clientes que necesitan ayuda para solucionar problemas del proceso de registro de unirse a Azure AD híbrido en circunstancias de trabajo remoto.

**Entorno de autenticación en la nube (mediante la sincronización hash de contraseña de Azure AD o la autenticación de paso a través)**

Este flujo de registro también se conoce como "Combinación de sincronización".

Este es un desglose de lo que sucede durante el proceso de registro:

1. Windows 10 detecta el registro de punto de conexión de servicio (SCP) cuando el usuario inicia sesión en el dispositivo.

    1. En primer lugar, el dispositivo intenta recuperar la información del inquilino de SCP del lado cliente en el Registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obtener más información, vea [el documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Si se produce un error, el dispositivo se comunica con Active Directory local para obtener información del espacio empresarial de SCP. Para comprobar SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Se recomienda habilitar SCP en Active Directory y solo usar SCP del lado cliente para la validación inicial.

2. Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD.

    Puedes comprobar si el dispositivo puede tener acceso a los recursos de Microsoft en la cuenta del sistema mediante el [script Probar conectividad de registro de dispositivos](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en Active Directory local. Esto requiere una línea de visión para el controlador de dominio.

4. El objeto Device que tiene certificado se sincroniza con Azure AD a través de Azure AD Conectar. El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Conectar. Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. En esta fase, debería poder ver el dispositivo de asunto en estado **"Pendiente"** en Hoja de dispositivo de Azure Portal.

6. En el siguiente inicio de sesión del Windows 10, se completará el registro.

    > [!NOTE]
    > Si está en VPN y el cierre de sesión o el inicio de sesión finaliza la conectividad del dominio, puede desencadenar el registro manualmente. Para ello:
    >
    > Emita `dsregcmd /join` un mensaje local en el símbolo del sistema o de forma remota a través de PSExec a su EQUIPO.
    >
    > Por ejemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Para ver problemas comunes con el Azure Active Directory de dispositivos, consulta [Preguntas más frecuentes sobre dispositivos.](https://docs.microsoft.com/azure/active-directory/devices/faq)
