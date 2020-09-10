---
title: El lote de migración de la carpeta pública no completado, se muestra sincronizado.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406610"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="39a95-102">El lote de migración de la carpeta pública no completado, se muestra sincronizado.</span><span class="sxs-lookup"><span data-stu-id="39a95-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="39a95-103">Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando “Sincronizado” por mucho tiempo.</span><span class="sxs-lookup"><span data-stu-id="39a95-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="39a95-104">Este es el comportamiento esperado.</span><span class="sxs-lookup"><span data-stu-id="39a95-104">This is expected behavior.</span></span>

<span data-ttu-id="39a95-105">Es habitual que el estado del lote de migración permanezca como Sincronizado durante algunas horas, antes de que cambie a Completando.</span><span class="sxs-lookup"><span data-stu-id="39a95-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="39a95-106">En el caso de las migraciones que impliquen un número grande de buzones objetivo, es normal que el estado permanezca en estado Sincronizado por más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de la carpeta pública subyacente haya fallado ni esté en cuarentena.</span><span class="sxs-lookup"><span data-stu-id="39a95-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="39a95-107">Permita un lapso de 24 a 48 horas para que el lote de migración finalice las tareas.</span><span class="sxs-lookup"><span data-stu-id="39a95-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
