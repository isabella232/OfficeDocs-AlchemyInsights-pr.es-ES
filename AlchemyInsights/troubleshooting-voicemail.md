---
title: 'Solución de problemas de correo de voz '
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
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608021"
---
# <a name="troubleshooting-voicemail"></a>Solución de problemas de correo de voz

Asegúrese de que la característica ocupado en ocupado es intencionada.

Si esta característica no es necesaria para este usuario:

1. Vaya al [centro de administración de Teams](https://admin.teams.microsoft.com/policies/calling).
1. En el raíl izquierdo, navegar por  >  **las directivas**  >  de llamadas de voz **administra directivas** en la **Directiva de llamadas**.
1. Seleccione **administrar usuarios**.
1. Buscar usuario y cambiar la Directiva de llamada a una que tiene **ocupado el ocupado está disponible cuando en una llamada** a **desactivado**.
1. Haga clic en **Aplicar**.
> [!NOTE]
> Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.

Para obtener más información sobre esta característica, consulte: [ocupado en ocupado está disponible mientras hay una llamada](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
