---
title: Los indicadores no funcionan mediante el explorador Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651512"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="ebe72-102">Los indicadores no funcionan mediante el explorador Edge</span><span class="sxs-lookup"><span data-stu-id="ebe72-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="ebe72-103">Después de crear un indicador, Edge (SmartScreen) no lo respetará.</span><span class="sxs-lookup"><span data-stu-id="ebe72-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="ebe72-104">Para obtener más información, consulte [Crear indicadores de direcciones IP y URL/dominios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="ebe72-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="ebe72-105">Paso 1: Asegúrese de lo siguiente</span><span class="sxs-lookup"><span data-stu-id="ebe72-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="ebe72-106">Compruebe que el indicador sea correcto (sin errores tipográficos en las direcciones IP/URL, la acción es correcta, los grupos RBAC son correctos).</span><span class="sxs-lookup"><span data-stu-id="ebe72-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="ebe72-107">Espere al menos dos horas después de crear el indicador para tener en cuenta cualquier posible latencia.</span><span class="sxs-lookup"><span data-stu-id="ebe72-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="ebe72-108">Confirme que los sistemas estén integrados en Microsoft Defender para punto de conexión.</span><span class="sxs-lookup"><span data-stu-id="ebe72-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="ebe72-109">Compruebe que los sistemas se puedan comunicar con la nube.</span><span class="sxs-lookup"><span data-stu-id="ebe72-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="ebe72-110">Compruebe que la pantalla inteligente esté habilitada y sea accesible yendo al [sitio de prueba](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="ebe72-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="ebe72-111">Paso 2: Solucionar el posible problema</span><span class="sxs-lookup"><span data-stu-id="ebe72-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="ebe72-112">Asegúrese de que el cliente cumpla los requisitos.</span><span class="sxs-lookup"><span data-stu-id="ebe72-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="ebe72-113">Para obtener más información, consulte [Crear indicadores de direcciones IP y URL/dominios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="ebe72-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="ebe72-114">Asegúrese de estar ejecutando la última versión del explorador Edge.</span><span class="sxs-lookup"><span data-stu-id="ebe72-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="ebe72-115">Para conocer la versión más reciente, consulte [Averiguar cuál versión de Microsoft Edge tiene](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="ebe72-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="ebe72-116">Reinicie el explorador Edge.</span><span class="sxs-lookup"><span data-stu-id="ebe72-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="ebe72-117">Vaya a un sitio para el que tenga configurado un indicador.</span><span class="sxs-lookup"><span data-stu-id="ebe72-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="ebe72-118">Si el sitio no aparece como se esperaba, continúe con el paso 3.</span><span class="sxs-lookup"><span data-stu-id="ebe72-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="ebe72-119">Paso 3: Recopilar datos</span><span class="sxs-lookup"><span data-stu-id="ebe72-119">Step 3: Collect data</span></span>

- <span data-ttu-id="ebe72-120">Recopilar los datos de diagnóstico de **MDEClientAnalyzer**.</span><span class="sxs-lookup"><span data-stu-id="ebe72-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="ebe72-121">Para obtener instrucciones, consulte [Problemas con los equipos de incorporación para Microsoft Defender para punto de conexión](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="ebe72-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="ebe72-122">Si está cómodo con la instalación y recopilación de un seguimiento de Fiddler, consulte [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="ebe72-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="ebe72-123">Si prefiere recibir instrucciones del Soporte técnico de Microsoft, seleccione el icono de Soporte que aparece a continuación para abrir un caso de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="ebe72-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
