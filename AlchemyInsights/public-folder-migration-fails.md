---
title: Error en la migración de carpetas públicas al 95%
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
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662426"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="aa612-102">Error en la migración de carpetas públicas al 95%</span><span class="sxs-lookup"><span data-stu-id="aa612-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="aa612-103">Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando **Sincronizado** durante un tiempo largo.</span><span class="sxs-lookup"><span data-stu-id="aa612-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="aa612-104">Este es el comportamiento que se espera.</span><span class="sxs-lookup"><span data-stu-id="aa612-104">This is expected behavior.</span></span>

<span data-ttu-id="aa612-105">Es habitual que el estado de un lote de migración permanezca como **Sincronizado** durante unas horas antes de que cambie a **Completando**.</span><span class="sxs-lookup"><span data-stu-id="aa612-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="aa612-106">En el caso de las migraciones que impliquen un gran número de buzones de destino, es normal que el estado permanezca en estado sincronizado durante más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de carpeta pública subyacente falle o se ponga en cuarentena.</span><span class="sxs-lookup"><span data-stu-id="aa612-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="aa612-107">Deje que el lote de migración finalice las 24/48 horas para completar las tareas.</span><span class="sxs-lookup"><span data-stu-id="aa612-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="aa612-108">En caso de que falle la migración de carpetas públicas al 95 %, con el error FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="aa612-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="aa612-109">Descargue y ejecute el script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) en el servidor local de Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa612-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="aa612-110">Ejecute las acciones correctivas que sugiere el script.</span><span class="sxs-lookup"><span data-stu-id="aa612-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="aa612-111">Ejecute la sincronización-MailPublicFolders (para Exchange 2010) o Sync-ModernMailPublicFolders (para Exchange 2013 y versiones posteriores).</span><span class="sxs-lookup"><span data-stu-id="aa612-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="aa612-112">Reanude la migración de carpetas públicas.</span><span class="sxs-lookup"><span data-stu-id="aa612-112">Resume public folder migration.</span></span>
