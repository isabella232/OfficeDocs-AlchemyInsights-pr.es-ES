---
title: El icono de calendario no se muestra en el cliente de Microsoft Teams
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
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576620"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>El icono de calendario no se muestra en el cliente de Microsoft Teams

La ficha **calendario** en Microsoft Teams requiere acceso a un buzón de Exchange a través de los servicios web Exchange. El buzón de Exchange puede estar en línea o local. Para los usuarios en línea que no ven la ficha **calendario** , asegúrese [de que tienen licencia para un buzón de Exchange Online y el buzón de correo está habilitado](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Si los usuarios están hospedados en local, debe confirmar que la configuración híbrida es correcta. Use el [Asistente para la configuración híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar el problema. Tenga en cuenta que [Teams requiere Exchange 2016 CU3 o una versión superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Para obtener más información y pasos para la solución de problemas, consulte [solucionar problemas de interacción de Microsoft Teams y Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
