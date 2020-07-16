---
title: Problemas con la incorporación de equipos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139058"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="382d6-102">Problemas con la incorporación de equipos</span><span class="sxs-lookup"><span data-stu-id="382d6-102">Issues with onboarding machines</span></span>

<span data-ttu-id="382d6-103">Es posible que tenga problemas con la incorporación de equipos al servicio de MDATP.</span><span class="sxs-lookup"><span data-stu-id="382d6-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="382d6-104">Si puede obtener acceso al equipo del usuario final, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="382d6-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="382d6-105">Descargue la herramienta de diagnóstico [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="382d6-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="382d6-106">Extraiga y ejecute MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="382d6-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="382d6-107">Busque el registro de diagnóstico en la carpeta llamada MDATPClientAnalyzerResult, la misma carpeta en la que se ha descargado la herramienta de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="382d6-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="382d6-108">Revise el archivo de registro, MDATPClientAnalyzer.txt, para buscar problemas de configuración del proxy de Internet o de conectividad.</span><span class="sxs-lookup"><span data-stu-id="382d6-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>