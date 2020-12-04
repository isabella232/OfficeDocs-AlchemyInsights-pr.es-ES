---
title: Solucionar un problema de PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571973"
---
# <a name="troubleshoot-prt-issue"></a>Solucionar un problema de PRT

Para que cualquier dispositivo finalice su autenticación, debe estar completamente registrado y en buen estado y poder adquirir un token de actualización principal (PRT).

El proceso de registro de Unión híbrida de Azure AD requiere que los dispositivos estén en una red corporativa. También funciona con VPN, pero hay algunas advertencias. Hemos escuchado a los clientes que necesitan asistencia para solucionar problemas del proceso de registro de Unión híbrida de Azure AD en circunstancias laborales remotas. A continuación, se muestra un desglose de lo que sucede ' en el parasol ' durante el proceso de registro.

**Entorno de autenticación en la nube (mediante la sincronización de hash de contraseña de Azure AD o la autenticación de paso a través)**

Este flujo de registro también se conoce como "sincronización de sincronización".

1. Windows 10 descubre un registro SCP cuando el usuario inicia sesión en el dispositivo.
    1. En primer lugar, el dispositivo intenta recuperar información de inquilinos del SCP del lado cliente en el registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para obtener más información, vea este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Si se produce un error, el dispositivo se comunica con Active Directory local (AD) para obtener la información de inquilino del punto de conexión de servicio (SCP). Para comprobar el SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Se recomienda habilitar SCP en AD y usar el SCP del lado cliente para la validación inicial.

2. Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD. Puede comprobar si el dispositivo puede tener acceso a los recursos de Microsoft en la cuenta del sistema mediante el script de conectividad de registro de dispositivos de prueba.

3. Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en AD local. Esto requiere línea de vista a controlador de dominio.

4. Un objeto de dispositivo que tiene un certificado se sincroniza con Azure AD a través de Azure AD Connect. El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Connect. Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. En esta fase, debería poder ver el dispositivo de asunto en el estado "pendiente" en la hoja de dispositivos de Azure portal.

6. El registro se completará en el siguiente inicio de sesión de usuario en Windows 10. 

> [!NOTE]
> Si está en VPN y un proceso de inicio de sesión con cierre de sesión finaliza la Conectividad del dominio, puede desencadenar el registro manualmente:
 1. Emita un dsregcmd/join localmente en el símbolo del administrador o de forma remota a través de PSExec en su PC. Por ejemplo, PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. Para obtener más información sobre problemas de combinaciones híbridas, consulte solucionar problemas de [dispositivos](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
