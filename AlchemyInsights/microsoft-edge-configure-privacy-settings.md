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
# <a name="microsoft-edge-configure-privacy-settings"></a>Configurar las opciones de privacidad de Microsoft Edge

De forma predeterminada, si Microsoft Edge se implementa en plataformas que no son Windows, los datos de diagnóstico y la información del sitio no se envían a Microsoft. Sin embargo, si Microsoft Edge se implementa en Windows 10, los datos de diagnóstico y la información del sitio se envían según la [configuración de datos de diagnóstico de Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)de los usuarios.

Para configurar la forma en que Microsoft Edge controla la recopilación de datos para su organización, use las siguientes directivas de Grupo:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): esta directiva permite informar sobre los datos de uso y relacionados con el bloqueo.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): esta directiva envía información del sitio que se usa para mejorar los servicios de Microsoft.

Para obtener más información, consulte [establecer la configuración](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)de las directivas.