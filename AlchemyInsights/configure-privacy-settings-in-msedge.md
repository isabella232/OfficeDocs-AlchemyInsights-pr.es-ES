---
title: Configuración de la privacidad en Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403857"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="94d66-102">Configuración de la privacidad en Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="94d66-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="94d66-103">De forma predeterminada, si Microsoft Edge se implementa en plataformas que no son de Windows, los datos de diagnóstico y la información del sitio no se envían a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="94d66-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="94d66-104">Sin embargo, si Microsoft Edge se implementa en Windows 10, los datos de diagnóstico y la información del sitio se envían de acuerdo con la configuración de datos [de diagnóstico de Windows de los usuarios.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="94d66-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="94d66-105">Para configurar el modo en que Microsoft Edge administra la recopilación de datos para su organización, use las siguientes directivas de grupo:</span><span class="sxs-lookup"><span data-stu-id="94d66-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="94d66-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) activa los informes de uso y datos relacionados con bloqueos.</span><span class="sxs-lookup"><span data-stu-id="94d66-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="94d66-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) envía la información del sitio usada para mejorar los servicios de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="94d66-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="94d66-108">Para obtener más información, vea [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="94d66-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
