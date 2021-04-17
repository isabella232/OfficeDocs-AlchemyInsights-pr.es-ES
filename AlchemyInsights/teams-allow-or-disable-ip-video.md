---
title: Teams permite o deshabilita el vídeo IP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826360"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="87b97-102">Teams permite o deshabilita el vídeo IP</span><span class="sxs-lookup"><span data-stu-id="87b97-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="87b97-103">**Cambiar o crear una directiva de reunión**</span><span class="sxs-lookup"><span data-stu-id="87b97-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="87b97-104">Para cambiar o crear una directiva de reuniones, vaya al **Centro de administración de Microsoft Teams > Reuniones > Directivas de reuniones**.</span><span class="sxs-lookup"><span data-stu-id="87b97-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="87b97-105">Seleccione una directiva de la lista o haga clic en **Agregar**.</span><span class="sxs-lookup"><span data-stu-id="87b97-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="87b97-106">Si va a crear una nueva directiva, agregue un nombre y una descripción.</span><span class="sxs-lookup"><span data-stu-id="87b97-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="87b97-107">El nombre no puede contener caracteres especiales ni tener más de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="87b97-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="87b97-108">Elija la configuración y, después, haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="87b97-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="87b97-109">Por ejemplo, supongamos que tiene muchos usuarios y quiere limitar el ancho de banda que necesitaría la reunión.</span><span class="sxs-lookup"><span data-stu-id="87b97-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="87b97-110">Cree una nueva directiva personalizada denominada "ancho de banda limitado" y deshabilite las opciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="87b97-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="87b97-111">En **Audio y vídeo**:</span><span class="sxs-lookup"><span data-stu-id="87b97-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="87b97-112">Desactive Permitir la grabación en la nube.</span><span class="sxs-lookup"><span data-stu-id="87b97-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="87b97-113">Desactive Permitir vídeo IP.</span><span class="sxs-lookup"><span data-stu-id="87b97-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="87b97-114">Luego asigne la directiva a los usuarios:</span><span class="sxs-lookup"><span data-stu-id="87b97-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="87b97-115">**Asignar una directiva de reunión a los usuarios**</span><span class="sxs-lookup"><span data-stu-id="87b97-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="87b97-116">En el panel de navegación izquierdo del Centro de administración de Microsoft Teams, vaya a **Usuarios** y, después, haga clic en el usuario.</span><span class="sxs-lookup"><span data-stu-id="87b97-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="87b97-117">Para seleccionar el usuario, haga clic a la izquierda del nombre de usuario y, después, en **Editar configuración**.</span><span class="sxs-lookup"><span data-stu-id="87b97-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="87b97-118">En **Directiva de reunión**, seleccione la directiva que quiera asignar y haga clic en **Aplicar**.</span><span class="sxs-lookup"><span data-stu-id="87b97-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="87b97-119">Para más información, consulte [Administrar directivas de reunión en Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="87b97-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
