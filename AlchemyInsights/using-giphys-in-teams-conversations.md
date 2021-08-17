---
title: Uso de Giphys en Teams conversaciones
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104325"
---
# <a name="using-giphys-in-teams-conversations"></a>Uso de Giphys en Teams conversaciones

El acceso de Giphys en Teams chat está habilitado de forma predeterminada. Como administrador, puede controlar si Giphys está [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) disponible para los usuarios estableciendo una directiva de mensajería y asegurándose de que **Usar Giphys** en conversaciones es **On**.

Si los GIF no funcionan como se esperaba en Teams conversaciones, compruebe:

La [directiva de mensajería](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) debe permitir Giphys. Para comprobarlo mediante cmdlets de PowerShell:

- Compruebe que puede [administrar Teams con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Ejecute el comando de PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) y compruebe que **AllowGiphy** está establecido en **TRUE**.
- Si **AllowGiphy está** establecido en **FALSE**, ejecute el siguiente comando de PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Las experiencias](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) conectadas opcionales deben habilitarse para permitir el acceso a la dirección URL de Giphy.

> [!NOTE]
> Si tiene varias directivas de mensajería de Teams configuradas para el inquilino, puede determinar la identidad de la directiva asignada al usuario afectado con el comando de PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Seleccione TeamsMessagingPolicy.
