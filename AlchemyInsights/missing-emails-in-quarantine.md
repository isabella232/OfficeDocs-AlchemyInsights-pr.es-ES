---
title: Falta correo electrónico en cuarentena
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
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831751"
---
# <a name="missing-emails-in-quarantine"></a>Falta correo electrónico en cuarentena"

Los administradores [pueden ver, liberar o eliminar estos mensajes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Para abrir el Centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) . Para abrir la página Cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Puede buscar según los siguientes valores:  

- **Id. de mensaje**: El identificador único global del mensaje. Si selecciona un mensaje en la lista, el  valor **id.** de mensaje aparece en el panel desplegable Detalles que aparece. Los administradores pueden usar [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para buscar mensajes y los valores de Id. de mensaje correspondientes.
- **Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.
- **Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.
- **Asunto**: Use el asunto completo del mensaje. La búsqueda no distingue entre mayúsculas y minúsculas.

Después de especificar los criterios de búsqueda, haga clic ![ en el botón Actualizar ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **para** filtrar los resultados.  

Los cmdlets que usa para ver y administrar mensajes y archivos en cuarentena son:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)tenga en cuenta que este cmdlet solo es para mensajes, no archivos de malware de ATP para SharePoint Online, OneDrive para la Empresa o Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)