---
title: Configurar las opciones de privacidad de Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599516"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="e0759-102">Configurar las opciones de privacidad de Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e0759-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="e0759-103">De forma predeterminada, si Microsoft Edge se implementa en plataformas que no son Windows, los datos de diagnóstico y la información del sitio no se envían a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e0759-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="e0759-104">Sin embargo, si Microsoft Edge se implementa en Windows 10, los datos de diagnóstico y la información del sitio se envían según la [configuración de datos de diagnóstico de Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)de los usuarios.</span><span class="sxs-lookup"><span data-stu-id="e0759-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="e0759-105">Para configurar la forma en que Microsoft Edge controla la recopilación de datos para su organización, use las siguientes directivas de Grupo:</span><span class="sxs-lookup"><span data-stu-id="e0759-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="e0759-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): esta directiva permite informar sobre los datos de uso y relacionados con el bloqueo.</span><span class="sxs-lookup"><span data-stu-id="e0759-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="e0759-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): esta directiva envía información del sitio que se usa para mejorar los servicios de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e0759-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="e0759-108">Para obtener más información, consulte [establecer la configuración](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)de las directivas.</span><span class="sxs-lookup"><span data-stu-id="e0759-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>