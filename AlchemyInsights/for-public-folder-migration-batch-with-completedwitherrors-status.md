---
title: Para el lote de migración de carpetas públicas con estado CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744130"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Para el lote de migración de carpetas públicas con estado CompletedWithErrors

Siga estos pasos para completar el lote y omitir los elementos incorrectos o grandes: 
1. Aprobar los elementos omitidos en el lote de migración:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Use el siguiente comando para aprobar los elementos omitidos en las solicitudes de migración que se han "sincronizado" pero que no se han completado:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. El lote de migración y las solicitudes deben reanudarse y completarse en unos minutos.

