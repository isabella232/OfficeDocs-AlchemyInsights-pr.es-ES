---
title: Configuración de directiva de reunión
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825460"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="60439-102">Administrar directivas de reuniones en Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="60439-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="60439-103">**Nota: Los cambios de directiva pueden tardar hasta 24 horas en tener efecto para los usuarios.**</span><span class="sxs-lookup"><span data-stu-id="60439-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="60439-104">Es posible que no pueda realizar cambios en las directivas recién creadas inmediatamente; espere 4 horas e intente modificar una directiva recién creada de nuevo.</span><span class="sxs-lookup"><span data-stu-id="60439-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="60439-105">Las directivas de reunión se usan para controlar las características que están disponibles para los participantes de las reuniones programadas por los usuarios de la organización.</span><span class="sxs-lookup"><span data-stu-id="60439-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="60439-106">Es posible que algunas características de directivas de reunión aún no se implementen en el Centro de administración de Teams (estas se etiquetan "próximamente" en la documentación).</span><span class="sxs-lookup"><span data-stu-id="60439-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="60439-107">En este caso, o si recibe un error como "No podemos actualizar la directiva en este momento pero volver a intentarlo más adelante" en el Centro de administración de Microsoft Teams, se recomienda usar PowerShell para crear o modificar directivas de reunión de Teams.</span><span class="sxs-lookup"><span data-stu-id="60439-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="60439-108">Para obtener más información acerca de las directivas de reunión, vea los siguientes recursos:</span><span class="sxs-lookup"><span data-stu-id="60439-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="60439-109">Para obtener información sobre cómo crear directivas, realizar cambios y asignar usuarios a la directiva, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="60439-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="60439-110">Para realizar cambios de directiva con cmdlets de PowerShell, vea [Información general de PowerShell de Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="60439-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="60439-111">Debe usar el módulo [de PowerShell de Skype Empresarial](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) para directivas de reuniones de Teams.</span><span class="sxs-lookup"><span data-stu-id="60439-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="60439-112">Revise la [documentación de los cmdlets \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="60439-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

