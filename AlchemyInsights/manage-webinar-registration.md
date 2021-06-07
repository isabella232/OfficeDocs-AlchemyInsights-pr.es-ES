---
title: Administrar el registro del seminario web
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783144"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="4862e-102">Administrar el registro del seminario web</span><span class="sxs-lookup"><span data-stu-id="4862e-102">Manage webinar registration</span></span>

<span data-ttu-id="4862e-103">Puede administrar quién puede registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams.</span><span class="sxs-lookup"><span data-stu-id="4862e-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="4862e-104">Para instalar PowerShell para Teams, consulte [PowerShell para Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="4862e-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="4862e-105">De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="4862e-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="4862e-106">Para permitir a cualquier usuario, incluidos usuarios anónimos, registrarse, debe establecer la directiva de reunión en **Todos** mediante el comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4862e-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="4862e-107">**Nota**: si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web.</span><span class="sxs-lookup"><span data-stu-id="4862e-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="4862e-108">Para más información y para habilitar esta configuración, consulte [Administrar la configuración de la reunión en Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="4862e-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="4862e-109">Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.</span><span class="sxs-lookup"><span data-stu-id="4862e-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="4862e-110">Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="4862e-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="4862e-111">Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="4862e-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
