---
title: Solución de problemas de importación de PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972436"
---
# <a name="troubleshooting-pst-import-issues"></a>Solución de problemas de importación de PST

- Si está importando dentro del propio cliente de Outlook, vea [Solucionar problemas al importar un archivo .pst de Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Si usa el servicio de importación y se atasca, tenga en cuenta que cada archivo PST que cargue en la ubicación de Azure Storage no debería ser superior a 20 GB. Los archivos PST de más de 20 GB pueden afectar al rendimiento del proceso de importación de PST. Para más información sobre la solución de problemas relacionados con trabajos atascados, consulte [Problemas que afectan a los trabajos de importación de PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Si quiere comprobar el estado de un trabajo de importación específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Para obtener detalles completos sobre el servicio de importación, consulte [Información general sobre la importación de archivos PST de su organización](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
