---
title: Cómo habilitar el correo de voz hospedado
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318665"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cómo habilitar el correo de voz hospedado

Para habilitar el correo de voz, **HostedVoicemail** debe establecerse en $true.

La **propiedad HostedVoicemail** del usuario mediante PowerShell remoto (RPS).

Para obtener más información sobre cómo conectarse a RPS, vea Microsoft Teams información general de [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obtener más información sobre cómo conectarse a RPS.

1. El administrador Teams debe iniciar sesión en PowerShell remoto para Teams.
1. Desde PowerShell, el administrador de Teams puede ejecutar **set-csuser user@contoso.com -HostedVoiceMail $true** donde el uri del sip es del usuario en cuestión.

**Nota:** Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.