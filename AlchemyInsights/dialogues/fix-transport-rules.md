---
title: Corregir reglas de transporte
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568681"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="f017d-102">Corregir reglas de transporte</span><span class="sxs-lookup"><span data-stu-id="f017d-102">Fix transport rules</span></span>

<span data-ttu-id="f017d-103">Una regla de flujo de correo personalizada afectó a este mensaje.</span><span class="sxs-lookup"><span data-stu-id="f017d-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="f017d-104">Para revisar la regla exacta, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f017d-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="f017d-105">En los resultados de envío, en **Información adicional**, anote el **GUID** o el nombre de **la directiva**.</span><span class="sxs-lookup"><span data-stu-id="f017d-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="f017d-106">Inicie el Shell de administración de Exchange.</span><span class="sxs-lookup"><span data-stu-id="f017d-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="f017d-107">Para obtener más información, vea [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="f017d-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="f017d-108">Ejecute este comando (mediante el GUID del envío):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="f017d-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="f017d-109">Revise la descripción para ver las condiciones configuradas que afectaron al mensaje.</span><span class="sxs-lookup"><span data-stu-id="f017d-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="f017d-110">Para obtener más información, [vea Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="f017d-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
