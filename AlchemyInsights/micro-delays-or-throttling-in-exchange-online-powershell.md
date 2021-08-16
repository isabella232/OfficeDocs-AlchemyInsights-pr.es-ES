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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098583"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro retrasos o limitación en Exchange Online PowerShell

Es posible que vea advertencias de "Micro retraso aplicado" o retrasos cuando ejecuta scripts y cmdlets en Exchange Online. Estas son algunas sugerencias sobre cómo solucionarlo:

- Ejecute nuestros diagnósticos para flexibilizar las directivas de limitación de PowerShell de su espacio empresarial. Esta solución resolverá el problema para la mayoría.
- Si el problema persiste, use el [módulo PowerShell de Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), que incluye CMDlets basados en la API de REST y que son mucho más eficaces. Esta podría ser una buena solución para muchos CMDlets Get- que se usan con frecuencia.
- Si necesita usar CMDlets que aún no están cubiertos en el módulo v2, vea [Ejecución de cmdlets de PowerShell para un gran número de usuarios en Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que habla de cómo evitar los límites de limitación de PowerShell en Exchange Online.
