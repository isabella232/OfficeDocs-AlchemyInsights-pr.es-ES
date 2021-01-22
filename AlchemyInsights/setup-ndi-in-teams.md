---
title: Activar la tecnología NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917321"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="af851-102">Activar la tecnología NDI</span><span class="sxs-lookup"><span data-stu-id="af851-102">Turn on NDI technology</span></span>

<span data-ttu-id="af851-103">La tecnología NDI requiere dos pasos para estar activados para un usuario:</span><span class="sxs-lookup"><span data-stu-id="af851-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="af851-104">El administrador del espacio empresarial debe habilitar la propiedad "AllowNDIStreaming" en CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="af851-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="af851-105">Una vez que se haya rellenado este cambio, el usuario final debe activar la tecnología NDI® para su cliente específico desde Configuración **> permisos.**</span><span class="sxs-lookup"><span data-stu-id="af851-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="af851-106">Para obtener más información, [vea Usar la tecnología NDI en Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="af851-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
