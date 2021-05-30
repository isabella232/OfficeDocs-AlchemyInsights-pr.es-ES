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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702143"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="3cd40-102">Micro retrasos o limitación en Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="3cd40-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="3cd40-103">Es posible que vea advertencias de "Micro retraso aplicado" o retrasos cuando ejecuta scripts y cmdlets en Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3cd40-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="3cd40-104">Estas son algunas sugerencias sobre cómo solucionarlo:</span><span class="sxs-lookup"><span data-stu-id="3cd40-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="3cd40-105">Ejecute nuestros diagnósticos para flexibilizar las directivas de limitación de PowerShell de su espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="3cd40-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="3cd40-106">Esta solución resolverá el problema para la mayoría.</span><span class="sxs-lookup"><span data-stu-id="3cd40-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="3cd40-107">Si el problema persiste, use el [módulo PowerShell de Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), que incluye CMDlets basados en la API de REST y que son mucho más eficaces.</span><span class="sxs-lookup"><span data-stu-id="3cd40-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="3cd40-108">Esta podría ser una buena solución para muchos CMDlets Get- que se usan con frecuencia.</span><span class="sxs-lookup"><span data-stu-id="3cd40-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="3cd40-109">Si necesita usar CMDlets que aún no están cubiertos en el módulo v2, vea [Ejecución de cmdlets de PowerShell para un gran número de usuarios en Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), que habla de cómo evitar los límites de limitación de PowerShell en Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="3cd40-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
