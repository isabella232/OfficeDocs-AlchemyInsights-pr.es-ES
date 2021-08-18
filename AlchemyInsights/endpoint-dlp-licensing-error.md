---
title: Error de licencia dlp de extremo
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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090172"
---
# <a name="endpoint-dlp-licensing-error"></a>Error de licencia DLP de extremo

Al intentar configurar DLP de extremo, si recibe el siguiente error:

`Your organization is missing the licenses required to manage these devices`.

Asegúrese de tener una de las siguientes suscripciones o complementos:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Cumplimiento de Microsoft 365 E5
- Cumplimiento de Microsoft 365 A5
- Gobierno y protección de información de Microsoft 365 E5
- Gobierno y protección de información de Microsoft 365 A5

> [!NOTE]
> Esto no funcionará para combinaciones de licencias como: Win E5 + O365 E5 + EMS E5. Debe tener una licencia pura de M365 E5 para configurar esta característica.

Para obtener más información sobre las licencias dlp de extremo, vea [Endpoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
