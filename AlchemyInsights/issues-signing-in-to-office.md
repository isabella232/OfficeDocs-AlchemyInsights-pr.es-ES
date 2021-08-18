---
title: Problemas al iniciar sesión en Microsoft 365 aplicaciones
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088053"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pantalla de inicio de sesión en blanco en Microsoft 365 aplicaciones

Para solucionar este problema, pruebe lo siguiente:
- Instale las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Restablecer opciones de Internet Explorer: ve a Herramientas Opciones de Internet Restablecimiento avanzado de  >    >    >  **Internet Explorer Configuración** (ten en cuenta que perderás la configuración personalizada) y, a continuación, intenta iniciar sesión en Office nuevo.
- Deshabilite Protección de aplicaciones de Windows Defender (WDAG) o cualquier firewall o programa antivirus similar:
    1. En el Panel de control, vaya **a Programas** y, a continuación, elija Activar o desactivar **Windows características.**
    2. Si Protección de aplicaciones de Windows Defender está habilitado, intente deshabilitarlo.<br/>
    **Nota:** Es posible que deba reiniciar el equipo.
- Asegúrese de que el complemento Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) no esté bloqueado por ninguna aplicación o programa antivirus o firewall.
- [Borra Office credenciales con](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Credential Manager.<br/>
    **Nota:** Las rutas de acceso del Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obtener más información, vea Connection [issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).