---
title: Problemas al iniciar sesión en aplicaciones de Microsoft 365
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833056"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Pantalla de inicio de sesión en blanco en aplicaciones de Microsoft 365

Para solucionar este problema, pruebe lo siguiente:
- Instalar las actualizaciones más recientes [para Windows](https://support.microsoft.com/help/4027667/windows-10-update) y [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Restablecer opciones de Internet Explorer: vaya a **Herramientas** Opciones de Internet Configuración avanzada de Internet Explorer (tenga en cuenta que perderá la configuración personalizada) y vuelva a intentar  >    >    >   iniciar sesión en Office.
- Deshabilite Windows Defender Protección de aplicaciones (WDAG) o cualquier firewall o programa antivirus similar:
    1. En el Panel de control, vaya **a Programas** y, a continuación, elija Activar o desactivar las características **de Windows.**
    2. Si Windows Defender Application Guard está habilitado, intenta deshabilitarlo.<br/>
    **Nota:** Es posible que deba reiniciar el equipo.
- Asegúrese de que el complemento Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) no esté bloqueado por ninguna aplicación o programa antivirus o firewall.
- [Borra las credenciales de Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) con el Administrador de credenciales de Windows.<br/>
    **Nota:** Las rutas de acceso del Registro para Office 2016 han cambiado a 16.0. (Por ejemplo: \Software\Microsoft\Office\16.0\Common\Identity\)

Para obtener más información, vea [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).