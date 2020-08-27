---
title: Error en la migración de carpetas públicas al 95%
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
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903620"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="dafa6-102">Error en la migración de carpetas públicas al 95%</span><span class="sxs-lookup"><span data-stu-id="dafa6-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="dafa6-103">En caso de que falle la migración de carpetas públicas al 95%, con el error FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="dafa6-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="dafa6-104">Descargue y ejecute el script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) en el servidor local de Exchange.</span><span class="sxs-lookup"><span data-stu-id="dafa6-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="dafa6-105">Ejecute las acciones correctivas que sugiere el script.</span><span class="sxs-lookup"><span data-stu-id="dafa6-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="dafa6-106">Ejecute la sincronización-MailPublicFolders (para Exchange 2010) o Sync-ModernMailPublicFolders (para Exchange 2013 y versiones posteriores).</span><span class="sxs-lookup"><span data-stu-id="dafa6-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="dafa6-107">Reanude la migración de carpetas públicas.</span><span class="sxs-lookup"><span data-stu-id="dafa6-107">Resume public folder migration.</span></span>
