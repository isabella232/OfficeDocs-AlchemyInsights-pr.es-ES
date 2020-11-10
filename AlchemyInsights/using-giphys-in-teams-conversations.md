---
title: Uso de Giphy en conversaciones de Microsoft Teams
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947536"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="2950f-102">Uso de Giphy en conversaciones de Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2950f-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="2950f-103">El acceso a giphy en el chat de Microsoft Teams está habilitado de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="2950f-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="2950f-104">Como administrador, puede controlar si Giphy están disponibles para los usuarios [estableciendo una directiva de mensajería](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) y garantizando que el **uso de giphy en conversaciones** esté **activado**.</span><span class="sxs-lookup"><span data-stu-id="2950f-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="2950f-105">Si los archivos GIF no funcionan como se esperaba en las conversaciones de Microsoft Teams, compruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="2950f-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="2950f-106">La [Directiva de mensajería](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) debe permitir giphy.</span><span class="sxs-lookup"><span data-stu-id="2950f-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="2950f-107">Para comprobar mediante cmdlets de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2950f-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="2950f-108">Compruebe que puede [administrar Teams con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="2950f-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="2950f-109">Ejecute el comando de PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) y compruebe que **AllowGiphy** está establecido en **true**.</span><span class="sxs-lookup"><span data-stu-id="2950f-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="2950f-110">Si **AllowGiphy** se establece en **false** , ejecute el siguiente comando de PowerShell [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="2950f-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="2950f-111">Las [experiencias opcionales conectadas](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) deben estar habilitadas para permitir el acceso a la dirección URL Giphy.</span><span class="sxs-lookup"><span data-stu-id="2950f-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="2950f-112">Si tiene varias directivas de mensajería de Microsoft Teams configuradas para el espacio empresarial, puede determinar la identidad de la directiva asignada al usuario afectado con el comando de PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Seleccione TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2950f-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
