---
title: Solución de problemas de importación de PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757757"
---
# <a name="troubleshooting-pst-import-issues"></a>Solución de problemas de importación de PST

- Si está importando desde el propio cliente de Outlook, consulte [Solucionar problemas al importar un archivo .pst de Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Si está usando el servicio de importación y está atascado, tenga en cuenta que cada archivo PST que cargue en la ubicación de Microsoft Azure Storage no debe ser mayor que 20 GB. Los archivos PST con un tamaño superior a 20 GB pueden afectar al rendimiento del proceso de importación de PST

- Si quiere comprobar el estado de un trabajo de importación específico, puede usar [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para más información sobre el servicio de importación, vea [Información general sobre la importación de archivos PST de su organización](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
