---
title: 'Solución de problemas de correo de voz '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608021"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="acc1f-102">Solución de problemas de correo de voz</span><span class="sxs-lookup"><span data-stu-id="acc1f-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="acc1f-103">Asegúrese de que la característica ocupado en ocupado es intencionada.</span><span class="sxs-lookup"><span data-stu-id="acc1f-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="acc1f-104">Si esta característica no es necesaria para este usuario:</span><span class="sxs-lookup"><span data-stu-id="acc1f-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="acc1f-105">Vaya al [centro de administración de Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="acc1f-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="acc1f-106">En el raíl izquierdo, navegar por  >  **las directivas**  >  de llamadas de voz **administra directivas** en la **Directiva de llamadas**.</span><span class="sxs-lookup"><span data-stu-id="acc1f-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="acc1f-107">Seleccione **administrar usuarios**.</span><span class="sxs-lookup"><span data-stu-id="acc1f-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="acc1f-108">Buscar usuario y cambiar la Directiva de llamada a una que tiene **ocupado el ocupado está disponible cuando en una llamada** a **desactivado**.</span><span class="sxs-lookup"><span data-stu-id="acc1f-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="acc1f-109">Haga clic en **Aplicar**.</span><span class="sxs-lookup"><span data-stu-id="acc1f-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="acc1f-110">Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.</span><span class="sxs-lookup"><span data-stu-id="acc1f-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="acc1f-111">Para obtener más información sobre esta característica, consulte: [ocupado en ocupado está disponible mientras hay una llamada](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="acc1f-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
