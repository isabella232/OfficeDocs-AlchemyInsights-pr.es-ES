---
title: Para lote de migración de carpetas públicas con estado CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812481"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="90e5f-102">Para lote de migración de carpetas públicas con estado CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="90e5f-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="90e5f-103">Siga estos pasos para completar el lote, omitiendo los elementos grandes o no:</span><span class="sxs-lookup"><span data-stu-id="90e5f-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="90e5f-104">Aprobar los elementos omitido en el lote de migración:</span><span class="sxs-lookup"><span data-stu-id="90e5f-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="90e5f-105">Use el siguiente comando para aprobar los elementos omitido en las solicitudes de migración que están "sincronizados" pero no completados:</span><span class="sxs-lookup"><span data-stu-id="90e5f-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="90e5f-106">El lote de migración y las solicitudes deben reanudarse y completarse en unos minutos.</span><span class="sxs-lookup"><span data-stu-id="90e5f-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

