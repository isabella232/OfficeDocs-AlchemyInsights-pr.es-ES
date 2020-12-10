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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608877"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cómo habilitar el correo de voz hospedado

Para habilitar el correo de voz, **HostedVoicemail** debe establecerse en $true.

La propiedad **HostedVoicemail** del usuario mediante el uso de PowerShell remoto (RPS).

Para obtener más información sobre cómo conectarse a RPS, vea información [General sobre PowerShell de Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obtener más información sobre cómo conectarse a RPS.

1. El administrador de Teams debe iniciar sesión en PowerShell remoto para Microsoft Teams.
1. En el símbolo del sistema de PowerShell, el administrador de Teams puede ejecutar **set-csuser user@contoso.com-HostedVoiceMail $true** donde el URI del SIP es del usuario en cuestión.

> [!NOTE]
> Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.