---
title: Mensajes de correo electrónico que faltan en cuarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673731"
---
# <a name="missing-emails-in-quarantine"></a>Mensajes que faltan en cuarentena

Los administradores pueden [ver, liberar o eliminar estos mensajes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir el centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) . Para abrir la página de cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puede buscar según los siguientes valores:  

- **Id. de mensaje**: El identificador único global del mensaje. Si selecciona un mensaje de la lista, el valor del  **identificador de mensaje**  aparece en el panel flotante de  **detalles**  que aparece. Los administradores pueden usar [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para buscar mensajes y los valores de Id. de mensaje correspondientes.
- **Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.
- **Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.
- **Asunto**: Use el asunto completo del mensaje. La búsqueda no distingue entre mayúsculas y minúsculas.

Una vez que haya introducido los criterios de búsqueda, haga clic en ![ Actualizar botón ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualizar** para filtrar los resultados.  

Los cmdlets que se usan para ver y administrar mensajes y archivos en cuarentena son los siguientes:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Vista previa de QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): tenga en cuenta que este cmdlet solo es para los mensajes, no para los archivos de malware de ATP para SharePoint Online, OneDrive para la empresa o Teams.
- [Versión-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)