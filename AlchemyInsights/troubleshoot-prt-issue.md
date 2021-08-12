---
title: Solucionar problemas de PRT
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972733"
---
# <a name="troubleshoot-prt-issue"></a>Solucionar problemas de PRT

Para que cualquier dispositivo complete la autenticación, debe estar totalmente registrado y en buen estado y poder adquirir un token de actualización principal (PRT).

El proceso híbrido de registro de unión a Azure AD requiere que los dispositivos se unan a una red corporativa. También funciona a través de VPN, pero hay algunas advertencias al respecto. Hemos escuchado a los clientes que necesitan ayuda para solucionar problemas del proceso de registro de unirse a Azure AD híbrido en circunstancias de trabajo remoto. Este es un desglose de lo que está sucediendo "debajo del capó" durante el proceso de registro.

**Entorno de autenticación en la nube (mediante la sincronización hash de contraseña de Azure AD o la autenticación de paso a través)**

Este flujo de registro también se conoce como "Combinación de sincronización".

1. Windows 10 detecta un registro SCP al iniciar sesión en el dispositivo.
    1. En primer lugar, el dispositivo intenta recuperar la información del inquilino de SCP del lado cliente en el Registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Si se produce un error, el dispositivo se comunica con Active Directory (AD) local para obtener información del espacio empresarial del Punto de conexión de servicio (SCP). Para comprobar SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Se recomienda habilitar SCP en AD y solo usar SCP del lado cliente para la validación inicial.

2. Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD. Puedes comprobar si el dispositivo puede acceder a los recursos de Microsoft en la cuenta del sistema mediante el script Probar conectividad de registro de dispositivos.

3. Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en AD local. Esto requiere una línea de visión para el controlador de dominio.

4. Un objeto de dispositivo que tiene un certificado se sincroniza con Azure AD a través de Azure AD Conectar. El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Conectar. Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. En esta fase, debería poder ver el dispositivo de asunto en estado "Pendiente" en la hoja Dispositivo de Azure Portal.

6. En el siguiente inicio de sesión del Windows 10, se completará el registro. 

> [!NOTE]
> Si está en VPN y un proceso de inicio de sesión finaliza la conectividad de dominio, puede desencadenar el registro manualmente:
 1. Emita un dsregcmd /join localmente en el símbolo del sistema de administración o de forma remota a través de PSExec a su PC. Por ejemplo, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Para obtener más información sobre los problemas de unión híbrida, consulta [Solucionar problemas de dispositivos.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
