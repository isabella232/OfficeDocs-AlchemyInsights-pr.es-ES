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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798661"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="9f7f7-102">Administrar el registro del seminario web</span><span class="sxs-lookup"><span data-stu-id="9f7f7-102">Manage webinar registration</span></span>

<span data-ttu-id="9f7f7-103">Puede administrar quién puede registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams.</span><span class="sxs-lookup"><span data-stu-id="9f7f7-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="9f7f7-104">Para instalar PowerShell para Teams, consulte [PowerShell para Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="9f7f7-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="9f7f7-105">De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **Todos**.</span><span class="sxs-lookup"><span data-stu-id="9f7f7-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="9f7f7-106">Si no ve la opción para permitir el registro para todos los usuarios en la invitación de reunión, vuelva a ejecutar la configuración *WhoCanRegister* para todos y espere 24 horas.</span><span class="sxs-lookup"><span data-stu-id="9f7f7-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="9f7f7-107">Para volver a ejecutar *WhoCanRegister*, use el comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9f7f7-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="9f7f7-108">**Nota**: si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web.</span><span class="sxs-lookup"><span data-stu-id="9f7f7-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="9f7f7-109">Para más información y para habilitar esta configuración, consulte [Administrar la configuración de la reunión en Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="9f7f7-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="9f7f7-110">Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.</span><span class="sxs-lookup"><span data-stu-id="9f7f7-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="9f7f7-111">Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="9f7f7-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="9f7f7-112">Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="9f7f7-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
