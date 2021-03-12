---
title: Solucionar problemas de forma remota con la incorporación de dispositivos Windows 10 a la Protección contra amenazas avanzada de Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737703"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="5c413-102">Solucionar problemas de forma remota con la incorporación de dispositivos Windows 10 a la Protección contra amenazas avanzada de Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="5c413-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="5c413-103">Si puede tener acceso al equipo remoto, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="5c413-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="5c413-104">Descargue la herramienta de diagnóstico [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).</span><span class="sxs-lookup"><span data-stu-id="5c413-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="5c413-105">Extraiga y ejecute MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="5c413-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="5c413-106">Busque el registro de diagnóstico en la carpeta MDATPClientAnalyzerResult, que es la misma carpeta donde se descargó la herramienta Analizador.</span><span class="sxs-lookup"><span data-stu-id="5c413-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="5c413-107">Para encontrar problemas con la configuración de proxy de Internet o conectividad, revise el archivo de registro MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="5c413-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="5c413-108">Para obtener más información, vea [Problemas con las máquinas de incorporación.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="5c413-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
