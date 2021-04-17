---
title: Micro retrasos o limitación en Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830050"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro retrasos o limitación en Exchange Online PowerShell

Es posible que vea advertencias de "Micro retraso aplicado" o retrasos cuando ejecuta scripts y cmdlets en Exchange Online. Aquí tiene dos sugerencias relacionadas con esto:

- Es posible que quiera usar el [módulo de PowerShell de Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), que incluye CMDlets basados en la API de REST y son significativamente más eficaces Esta podría ser una buena solución para muchos CMDlets Get- que se usan con frecuencia.
- Si necesita usar CMDlets que aún no están cubiertos en el módulo v2, consulte [Ejecución de cmdlets de PowerShell para un gran número de usuarios en Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que habla sobre cómo sortear la limitación esperada de PowerShell en Exchange Online.
