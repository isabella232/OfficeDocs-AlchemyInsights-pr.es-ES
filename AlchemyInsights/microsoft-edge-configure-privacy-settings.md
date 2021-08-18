---
title: Microsoft Edge configuración de privacidad
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114189"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configuración de privacidad

De forma predeterminada, si Microsoft Edge se implementa en plataformas no Windows, los datos de diagnóstico y la información del sitio no se envían a Microsoft. Sin embargo, si Microsoft Edge se implementa en Windows 10, los datos de diagnóstico y la información del sitio se envían de acuerdo con la configuración Windows [datos de diagnóstico de los usuarios.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Para configurar cómo Microsoft Edge la recopilación de datos para su organización, use las siguientes directivas de grupo:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)esta directiva permite informar sobre el uso y los datos relacionados con bloqueos.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)esta directiva envía información del sitio que se usa para mejorar servicios Microsoft.

Para obtener más información, vea [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).