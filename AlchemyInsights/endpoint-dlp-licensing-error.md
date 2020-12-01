---
title: Error de licencias de DLP de punto de conexión
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477703"
---
# <a name="endpoint-dlp-licensing-error"></a>Error de licencias de DLP de punto de conexión

Al intentar configurar la DLP de los extremos, si recibe el siguiente error:

`Your organization is missing the licenses required to manage these devices`.

Asegúrese de que dispone de una de las siguientes suscripciones o complementos:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Cumplimiento de Microsoft 365 E5
- Cumplimiento de Microsoft 365 A5
- Gobierno y protección de información de Microsoft 365 E5
- Gobierno y protección de información de Microsoft 365 A5

> [!NOTE]
> Esto no funcionará para las combinaciones de licencia como: Win E5 + O365 E5 + EMS E5. Debe tener una licencia pura de M365 E5 para configurar esta característica.

Para obtener más información sobre licencias de DLP de terminal, consulte [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
