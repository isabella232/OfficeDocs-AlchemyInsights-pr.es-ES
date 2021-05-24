---
title: Solucionar los errores de retención de eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583762"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="86fdc-102">Solucionar los errores de retención de eDiscovery</span><span class="sxs-lookup"><span data-stu-id="86fdc-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="86fdc-103">¿Está teniendo problemas con las retenciones de eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="86fdc-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="86fdc-104">Estos son algunos procedimientos recomendados que puede probar:</span><span class="sxs-lookup"><span data-stu-id="86fdc-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="86fdc-105">Compruebe el estado de distribución de retención.</span><span class="sxs-lookup"><span data-stu-id="86fdc-105">Check the hold distribution status.</span></span>  <span data-ttu-id="86fdc-106">Si el estado es **Activado (pendiente)** o **Desactivado (pendiente)**, espere a que se complete la distribución de la retención.</span><span class="sxs-lookup"><span data-stu-id="86fdc-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="86fdc-107">Combine las actualizaciones de retención de eDiscovery en una sola solicitud en masa en lugar de actualizar la directiva repetidamente para cada transacción.</span><span class="sxs-lookup"><span data-stu-id="86fdc-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="86fdc-108">Ejecute Set-CaseHoldPolicy <policyname> -RetryDistribution en el Powershell del Centro de seguridad y cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="86fdc-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="86fdc-109">Para más información, consulte [Conectarse al PowerShell del Centro de seguridad y cumplimiento](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="86fdc-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="86fdc-110">Para ver los pasos para comprobar esta configuración y los procedimientos recomendados adicionales para mitigar y resolver problemas de retención de eDiscovery, vea [Solucionar problemas de retención de eDiscovery](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="86fdc-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="86fdc-111">Para obtener información sobre cómo solucionar otros problemas comunes de eDiscovery, consulte [Investigar y solucionar comunes de eDiscovery](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="86fdc-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
