---
title: Habilitar los seminarios web de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760858"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="bc3f4-102">Habilitar los seminarios web de Teams</span><span class="sxs-lookup"><span data-stu-id="bc3f4-102">Enable Teams Webinars</span></span>

<span data-ttu-id="bc3f4-103">Los seminarios web están habilitados de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-103">Webinars are enabled by default.</span></span> <span data-ttu-id="bc3f4-104">Puede administrar quién puede programar y registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="bc3f4-105">Todos los usuarios que puedan crear una reunión también podrán crear una reunión de seminario web.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="bc3f4-106">Si quiere administrar quién puede programar los seminarios web de Teams, use *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="bc3f4-107">De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **Todos**.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="bc3f4-108">Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="bc3f4-109">Para cambiar esta configuración, debe instalar [PowerShell de Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="bc3f4-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="bc3f4-110">Además, las directivas de la reunión aplican para los seminarios web de Teams.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="bc3f4-111">Por ejemplo, si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="bc3f4-112">Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="bc3f4-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="bc3f4-113">Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="bc3f4-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>