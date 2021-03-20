---
title: Problemas relacionados con la incorporación de equipos a Microsoft Defender para puntos de conexión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901584"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="37a88-102">Problemas relacionados con la incorporación de equipos a Microsoft Defender para puntos de conexión</span><span class="sxs-lookup"><span data-stu-id="37a88-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="37a88-103">Es posible que tenga problemas con la incorporación de equipos al servicio de MDE.</span><span class="sxs-lookup"><span data-stu-id="37a88-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="37a88-104">Si puede obtener acceso al equipo del usuario final, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="37a88-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="37a88-105">Descargue la última versión preliminar de la herramienta de diagnóstico [Analizador de clientes MDE](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="37a88-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="37a88-106">Haga clic con el botón derecho en **MDEClientAnalyzer.cmd** y seleccione "Ejecutar como administrador".</span><span class="sxs-lookup"><span data-stu-id="37a88-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="37a88-107">Siga las instrucciones sugeridas en **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="37a88-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="37a88-108">Para consultar registros más detallados, consulte la subcarpeta creada llamada **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="37a88-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="37a88-109">Si necesita instrucciones adicionales, contacte [Soporte técnico de Microsoft Defender para punto de conexión](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) y proporcione el archivo resultante MDEClientAnalyzerResult.zip para su análisis.</span><span class="sxs-lookup"><span data-stu-id="37a88-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
