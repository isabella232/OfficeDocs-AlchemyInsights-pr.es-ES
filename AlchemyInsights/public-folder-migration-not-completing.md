---
title: El lote de migración de la carpeta pública no completado, se muestra sincronizado.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771491"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="87541-102">El lote de migración de la carpeta pública no completado, se muestra sincronizado.</span><span class="sxs-lookup"><span data-stu-id="87541-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="87541-103">Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando “Sincronizado” por mucho tiempo.</span><span class="sxs-lookup"><span data-stu-id="87541-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="87541-104">Este es el comportamiento esperado.</span><span class="sxs-lookup"><span data-stu-id="87541-104">This is expected behavior.</span></span>

<span data-ttu-id="87541-105">Es habitual que el estado del lote de migración permanezca como Sincronizado durante algunas horas, antes de que cambie a Completando.</span><span class="sxs-lookup"><span data-stu-id="87541-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="87541-106">En el caso de las migraciones que impliquen un número grande de buzones objetivo, es normal que el estado permanezca en estado Sincronizado por más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de la carpeta pública subyacente haya fallado ni esté en cuarentena.</span><span class="sxs-lookup"><span data-stu-id="87541-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="87541-107">Permita un lapso de 24 a 48 horas para que el lote de migración finalice las tareas.</span><span class="sxs-lookup"><span data-stu-id="87541-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
