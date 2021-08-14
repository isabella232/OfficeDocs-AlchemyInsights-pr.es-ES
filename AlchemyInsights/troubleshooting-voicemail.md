---
title: 'Solución de problemas del correo de voz '
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
ms.openlocfilehash: e639d74cd8dbbb03ffb5b253451c99c8fe639f024a46e173845a0f4d322e43ca
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972400"
---
# <a name="troubleshooting-voicemail"></a>Solución de problemas de correo de voz

Asegúrese de que la característica Ocupado en ocupado es intencionada.

Si esta característica no es necesaria en este usuario:

1. Vaya a [Teams Centro de administración.](https://admin.teams.microsoft.com/policies/calling)
1. En el carril izquierdo, navegue **por las directivas de** llamadas de  >  **voz**  >  **Administrar directivas** en la directiva de **llamadas.**
1. Seleccione **Administrar usuarios**.
1. Buscar usuario y cambiar la directiva de llamada a una que tenga Ocupado en ocupado está **disponible cuando se realiza** una llamada a **Desactivado**.
1. Haga clic en **Aplicar**.
> [!NOTE]
> Los cambios en las directivas pueden tardar hasta 24 horas en replicarse.

Para obtener más información sobre esta característica, consulte: [Ocupado en ocupado está disponible mientras se llama a](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
