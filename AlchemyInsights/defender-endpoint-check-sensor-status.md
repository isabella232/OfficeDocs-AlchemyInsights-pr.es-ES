---
title: Estado de sensor de Microsoft Defender para punto de conexión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: 903d64a59d3bf870572c3c643e3d9cb801b571cb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321092"
---
# <a name="defender-endpoint-check-sensor-status"></a>Estado de sensor de Microsoft Defender para punto de conexión

El icono **Dispositivos con problemas de sensores** está en el panel Operaciones de seguridad. Este icono proporciona información sobre la capacidad de cada dispositivo de dar datos de sensores y comunicarse con el servicio Microsoft Defender para punto de conexión. Indica cuántos dispositivos requieren atención y le ayuda a identificar dispositivos problemáticos y tomar medidas para corregir los problemas conocidos.

Los dos indicadores de estado del icono dan información sobre el número de dispositivos que no informan correctamente al servicio:

- Dispositivos **mal configurados** que podrían informar parcialmente de datos del sensor al servicio Microsoft Defender para punto de conexión y que podrían tener errores de configuración que deban corregirse.
- **Dispositivos** inactivos que han dejado de informar al servicio Microsoft Defender para punto de conexión durante más de siete días en el mes pasado.

Al hacer clic en cualquiera de los grupos, se le dirigirá a la lista de dispositivos, filtrada según sus opciones. En la lista Dispositivos, puede filtrar la lista de estado según los siguientes estados:

- Dispositivos **activos** que informan de forma activa al servicio Microsoft Defender para punto de conexión.
- Dispositivos **mal configurados** que podrían informar parcialmente de datos del sensor al servicio Microsoft Defender para punto de conexión, pero que tienen errores de configuración que deben corregirse. Los dispositivos mal configurados pueden tener uno o varios de los siguientes problemas:

    - No hay datos de sensor: los dispositivos han dejado de enviar datos de sensores. Se pueden activar alertas limitadas desde el dispositivo.
    - Comunicaciones deficientes: la capacidad de comunicarse con el dispositivo es deficiente. Puede que el envío de archivos para un análisis profundo, el bloqueo de archivos, el aislamiento de dispositivo de la red y otras acciones que requieran comunicación con el dispositivo no funcionen.
- Dispositivos **inactivos** que han dejado de informar al servicio Microsoft Defender para punto de conexión.

Puede descargar toda la lista en formato CSV con la característica Exportar.

Para obtener más información, consulte [Comprobar el estado del sensor en Microsoft Defender para punto de conexión](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Para obtener más información sobre qué provocó que un dispositivo esté inactivo o mal configurado, vea [Corregir sensores en mal estado en Microsoft Defender para el punto de conexión](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
