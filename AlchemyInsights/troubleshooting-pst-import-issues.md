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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059832"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="e4c4e-102">Solución de problemas de importación de PST</span><span class="sxs-lookup"><span data-stu-id="e4c4e-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="e4c4e-103">Si está importando dentro del propio cliente de Outlook, vea [Solucionar problemas al importar un archivo .pst de Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="e4c4e-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="e4c4e-104">Si usa el servicio de importación y se atasca, tenga en cuenta que cada archivo PST que cargue en la ubicación de Azure Storage no debería ser superior a 20 GB.</span><span class="sxs-lookup"><span data-stu-id="e4c4e-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="e4c4e-105">Los archivos PST de más de 20 GB pueden afectar al rendimiento del proceso de importación de PST.</span><span class="sxs-lookup"><span data-stu-id="e4c4e-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="e4c4e-106">Para más información sobre la solución de problemas relacionados con trabajos atascados, consulte [Problemas que afectan a los trabajos de importación de PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="e4c4e-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="e4c4e-107">Si quiere comprobar el estado de un trabajo de importación específico, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="e4c4e-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="e4c4e-108">Para obtener detalles completos sobre el servicio de importación, consulte [Información general sobre la importación de archivos PST de su organización](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e4c4e-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
