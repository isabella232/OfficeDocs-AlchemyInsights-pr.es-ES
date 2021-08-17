---
title: Configurar DLP en punto de conexión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892816"
---
# <a name="configure-endpoint-dlp"></a>Configurar DLP en punto de conexión

DLP en punto de conexión de Microsoft le permite ampliar la funcionalidad de protección y supervisión de DLP a información confidencial en dispositivos con Windows 10. Después de que los dispositivos estén integrados en la administración de dispositivos, puede crear directivas DLP para aplicar acciones de protección en los elementos. El explorador de actividades se puede usar para supervisar la actividad de elementos confidenciales. Para más información, consulte [Incorporación de dispositivos en la administración de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Para empezar a usar DLP en punto de conexión:

- Asegúrese de que tiene la licencia de SKU o suscripciones adecuadas. Para más información, consulte [Licencia de SKU o suscripciones](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Compruebe los permisos necesarios para habilitar la administración de dispositivos, acceder a la página de incorporación o activar o desactivar la supervisión de dispositivos. Para más información, consulte [Permisos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Incorpore dispositivos en la Administración de dispositivos siguiendo el procedimiento de incorporación de dispositivos. Para más información, consulte [Incorporación de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Cree directivas DLP para proteger sus elementos confidenciales. Para más información, consulte [Escenarios de directiva DLP de los puntos de conexión](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Para más información sobre DLP en punto de conexión de Microsoft, consulte [Obtener información sobre la prevención de pérdida de datos en punto de conexión de Microsoft 365 (vista previa)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pasos importantes de recopilación de datos, si se necesita Soporte técnico:**

1. Descargue la [Versión preliminar de MDATP Client Analyzer](https://aka.ms/betamdatpanalyzer).
1. Ejecute la herramienta como administrador en la ventana de símbolo del sistema:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Cuando aparezca el mensaje **Escriba el número de minutos para recopilar seguimientos:**, escriba el número de minutos necesarios para ejecutar el escenario
1. Ejecute el escenario.

Recopile el archivo zip resultante para entregarlo al agente de soporte.
