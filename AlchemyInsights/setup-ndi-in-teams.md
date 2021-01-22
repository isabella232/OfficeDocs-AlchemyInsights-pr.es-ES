---
title: Activar la tecnología NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917321"
---
# <a name="turn-on-ndi-technology"></a>Activar la tecnología NDI

La tecnología NDI requiere dos pasos para estar activados para un usuario:

1. El administrador del espacio empresarial debe habilitar la propiedad "AllowNDIStreaming" en CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Una vez que se haya rellenado este cambio, el usuario final debe activar la tecnología NDI® para su cliente específico desde Configuración **> permisos.**

Para obtener más información, [vea Usar la tecnología NDI en Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
