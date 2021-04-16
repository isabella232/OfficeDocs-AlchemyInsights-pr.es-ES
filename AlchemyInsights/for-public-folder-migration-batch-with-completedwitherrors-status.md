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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para lote de migración de carpetas públicas con estado CompletedWithErrors

Siga estos pasos para completar el lote, omitiendo los elementos grandes o no: 
1. Aprobar los elementos omitido en el lote de migración:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Use el siguiente comando para aprobar los elementos omitido en las solicitudes de migración que están "sincronizados" pero no completados:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. El lote de migración y las solicitudes deben reanudarse y completarse en unos minutos.

