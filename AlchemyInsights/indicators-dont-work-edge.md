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
ms.openlocfilehash: 4094371ee0a3b3ec8d29454fd66f3e9e7c3f35a91b9ea05f308325bc447ce11c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926334"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Los indicadores no funcionan mediante el explorador Edge

Después de crear un indicador, Edge (SmartScreen) no lo respetará. Para obtener más información, consulte [Crear indicadores de direcciones IP y URL/dominios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Paso 1: Asegúrese de lo siguiente

- Compruebe que el indicador sea correcto (sin errores tipográficos en las direcciones IP/URL, la acción es correcta, los grupos RBAC son correctos).
- Espere al menos dos horas después de crear el indicador para tener en cuenta cualquier posible latencia.
- Confirme que los sistemas estén integrados en Microsoft Defender para punto de conexión.
- Compruebe que los sistemas se puedan comunicar con la nube.
- Compruebe que la pantalla inteligente esté habilitada y sea accesible yendo al [sitio de prueba](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Paso 2: Solucionar el posible problema

- Asegúrese de que el cliente cumpla los requisitos. Para obtener más información, consulte [Crear indicadores de direcciones IP y URL/dominios](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Asegúrese de estar ejecutando la última versión del explorador Edge. Para conocer la versión más reciente, consulte [Averiguar cuál versión de Microsoft Edge tiene](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Reinicie el explorador Edge.
- Vaya a un sitio para el que tenga configurado un indicador. Si el sitio no aparece como se esperaba, continúe con el paso 3. 

## <a name="step-3-collect-data"></a>Paso 3: Recopilar datos

- Recopilar los datos de diagnóstico de **MDEClientAnalyzer**. Para obtener instrucciones, consulte [Problemas con los equipos de incorporación para Microsoft Defender para punto de conexión](issues-with-onboarding-machines.md).
- Si está cómodo con la instalación y recopilación de un seguimiento de Fiddler, consulte [Telerik Fiddler](http://www.telerik.com/fiddler).
- Si prefiere recibir instrucciones del Soporte técnico de Microsoft, seleccione el icono de Soporte que aparece a continuación para abrir un caso de soporte técnico.
