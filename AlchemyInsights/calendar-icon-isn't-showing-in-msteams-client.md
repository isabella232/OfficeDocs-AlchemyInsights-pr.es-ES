---
title: El icono de calendario no se muestra en Microsoft Teams cliente
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120021"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>El icono de calendario no se muestra en Microsoft Teams cliente

La **pestaña** Calendario en Teams requiere acceso a un buzón Exchange mediante Exchange Web Services. El Exchange buzón de correo puede ser En línea o Local. Para los usuarios en línea que no ven **la** pestaña Calendario, asegúrese de que tienen licencia para un buzón de Exchange Online y que el buzón [está habilitado.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Si los usuarios están adosados localmente, debe confirmar que la configuración híbrida está en buen estado. Use el [Asistente para la configuración híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar el problema. Tenga en cuenta que [Teams requiere Exchange 2016 CU3 o una versión superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obtener más información y pasos de solución de problemas, [vea Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
