---
title: Omitir lobby
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820051"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="aaa9f-102">Controlar la configuración de la sala de espera y el nivel de participación en Teams</span><span class="sxs-lookup"><span data-stu-id="aaa9f-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="aaa9f-103">Si desea permitir que todos, incluidos los usuarios de acceso telefónico, externos y anónimos, omita la sala de **espera,** use PowerShell para realizar esta tarea.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="aaa9f-104">Este es un ejemplo de modificación de la directiva de reunión global para su organización.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="aaa9f-105">Actualmente, este cmdlet requiere el uso del módulo PowerShell de Skype Empresarial.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="aaa9f-106">Para configurarse para usar este cmdlet, consulte [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="aaa9f-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="aaa9f-107">Una vez que haya configurado una directiva, debe aplicarla a los usuarios; o, si ha modificado la directiva global, se aplicará automáticamente a los usuarios.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="aaa9f-108">Para cualquier cambio de directiva, debe esperar al menos 4 horas hasta **24** horas para que las directivas entren en vigor.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="aaa9f-109">Asegúrese de revisar la documentación siguiente antes de realizar estos cambios para comprender exactamente lo que esto permite.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="aaa9f-110">Descripción de los controles de directiva de la sala de espera de reuniones de Teams</span><span class="sxs-lookup"><span data-stu-id="aaa9f-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="aaa9f-111">Estos valores controlan qué participantes de la reunión esperan en la sala de espera antes de ser admitidos en la reunión y el nivel de participación que se les permite en una reunión.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="aaa9f-112">Puede usar PowerShell para actualizar la configuración de directiva de reunión que aún no se ha implementado (etiquetada "próximamente") en el Centro de administración de Teams.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="aaa9f-113">Vea a continuación un cmdlet de PowerShell de ejemplo que permite a todos los usuarios omitir la sala de espera.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="aaa9f-114">[Admitir automáticamente a las](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) personas es una directiva por organizador que controla si las personas se unen a una reunión directamente o esperan en la sala de espera hasta que un usuario autenticado los admita.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="aaa9f-115">[Permitir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) que personas anónimas inicien una reunión es una directiva por organizador que controla si las personas anónimas, incluidos B2B y los usuarios federados, pueden unirse a la reunión del usuario sin un usuario autenticado de la organización que asista.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="aaa9f-116">[Permitir](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) que los usuarios de acceso telefónico local omitan la sala de espera **(** próximamente ) es una directiva  por organizador que controla si las personas que marcan por teléfono se unen a la reunión directamente o esperan en la sala de espera independientemente de la configuración Admitir automáticamente personas.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="aaa9f-117">Permitir que los organizadores invalide la configuración de la sala de espera ( próximamente **)** es una directiva  por organizador que controla si el organizador de la reunión puede invalidar la configuración de la sala de espera que un administrador establece en Admitir automáticamente a las personas y Permitir que los usuarios de acceso telefónico local omitan la sala de espera cuando programe una nueva reunión. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) </span><span class="sxs-lookup"><span data-stu-id="aaa9f-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="aaa9f-118">**Nota:** Lea [Administrar directivas de reunión en Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) para obtener una introducción completa a las directivas de reunión de Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aaa9f-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
