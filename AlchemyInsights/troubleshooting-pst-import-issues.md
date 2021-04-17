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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826180"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="bbbd4-102">Solución de problemas de importación de PST</span><span class="sxs-lookup"><span data-stu-id="bbbd4-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="bbbd4-103">Si está importando desde el propio cliente de Outlook, consulte [Solucionar problemas al importar un archivo .pst de Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="bbbd4-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="bbbd4-104">Si está usando el servicio de importación y está atascado, tenga en cuenta que cada archivo PST que cargue en la ubicación de Microsoft Azure Storage no debe ser mayor que 20 GB.</span><span class="sxs-lookup"><span data-stu-id="bbbd4-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="bbbd4-105">Los archivos PST con un tamaño superior a 20 GB pueden afectar al rendimiento del proceso de importación de PST</span><span class="sxs-lookup"><span data-stu-id="bbbd4-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="bbbd4-106">Si quiere comprobar el estado de un trabajo de importación específico, puede usar [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="bbbd4-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="bbbd4-107">Para más información sobre el servicio de importación, vea [Información general sobre la importación de archivos PST de su organización](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="bbbd4-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
