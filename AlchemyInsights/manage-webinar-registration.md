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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760850"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="e2638-102">Administrar el registro del seminario web</span><span class="sxs-lookup"><span data-stu-id="e2638-102">Manage webinar registration</span></span>

<span data-ttu-id="e2638-103">Puede administrar quién puede registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams.</span><span class="sxs-lookup"><span data-stu-id="e2638-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="e2638-104">De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **Todos**.</span><span class="sxs-lookup"><span data-stu-id="e2638-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="e2638-105">Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.</span><span class="sxs-lookup"><span data-stu-id="e2638-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="e2638-106">Para cambiar esta configuración, debe instalar [PowerShell de Teams](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="e2638-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="e2638-107">Además, las directivas de la reunión aplican para los seminarios web de Teams.</span><span class="sxs-lookup"><span data-stu-id="e2638-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="e2638-108">Por ejemplo, si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web.</span><span class="sxs-lookup"><span data-stu-id="e2638-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="e2638-109">Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="e2638-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="e2638-110">Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="e2638-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>