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
# <a name="using-giphys-in-teams-conversations"></a>Uso de Giphy en conversaciones de Microsoft Teams

El acceso a giphy en el chat de Microsoft Teams está habilitado de forma predeterminada. Como administrador, puede controlar si Giphy están disponibles para los usuarios [estableciendo una directiva de mensajería](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) y garantizando que el **uso de giphy en conversaciones** esté **activado**.

Si los archivos GIF no funcionan como se esperaba en las conversaciones de Microsoft Teams, compruebe lo siguiente:

La [Directiva de mensajería](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) debe permitir giphy. Para comprobar mediante cmdlets de PowerShell:

- Compruebe que puede [administrar Teams con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Ejecute el comando de PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) y compruebe que **AllowGiphy** está establecido en **true**.
- Si **AllowGiphy** se establece en **false** , ejecute el siguiente comando de PowerShell [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Las [experiencias opcionales conectadas](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) deben estar habilitadas para permitir el acceso a la dirección URL Giphy.

> [!NOTE]
> Si tiene varias directivas de mensajería de Microsoft Teams configuradas para el espacio empresarial, puede determinar la identidad de la directiva asignada al usuario afectado con el comando de PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Seleccione TeamsMessagingPolicy.
