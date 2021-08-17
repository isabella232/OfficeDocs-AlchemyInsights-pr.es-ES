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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055571"
---
# <a name="how-to-enable-hosted-voicemail"></a>Cómo habilitar el correo de voz hospedado

Para habilitar el correo de voz, **HostedVoicemail** debe establecerse en $true.

La **propiedad HostedVoicemail** del usuario mediante PowerShell remoto (RPS).

Para obtener más información sobre cómo conectarse a RPS, vea Microsoft Teams información general de [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) para obtener más información sobre cómo conectarse a RPS.

1. El administrador Teams debe iniciar sesión en PowerShell remoto para Teams.
1. Desde PowerShell, el administrador de Teams puede ejecutar **set-csuser user@contoso.com -HostedVoiceMail $true** donde el uri del sip es del usuario en cuestión.

> [!NOTE]
> Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.