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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023539"
---
# <a name="turn-on-ndi-technology"></a>Activar la tecnología NDI

La tecnología NDI requiere dos pasos para estar activada para un usuario:

1. El administrador de inquilinos debe habilitar la propiedad "AllowNDIStreaming" en CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Una vez que se haya rellenado este cambio, el usuario final debe activar la tecnología NDI® para su cliente específico desde **Configuración > permisos**.

Para obtener más información, vea [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
