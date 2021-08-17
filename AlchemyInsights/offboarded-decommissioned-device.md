---
title: Problemas con la eliminación de un dispositivo fuera deborde o retirada del inventario de dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076689"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemas con la eliminación de un dispositivo fuera deborde o retirada del inventario de dispositivos

Actualmente, Microsoft Defender para endpoint no permite quitar manualmente el registro de dispositivo de un dispositivo fuera deborde o dado de baja del Inventario de dispositivos.

Por motivos de seguridad, el dispositivo permanece en el portal como un registro histórico hasta 180 días. Sin embargo, los datos del dispositivo se purgan según el período de retención configurado.

**Nota:** Un dispositivo fuera deborde o desmantelado cambia automáticamente al **estado inactivo** después de siete días. Además, los dispositivos que no están activos en los últimos 30 días no se tienen en cuenta en los datos que reflejan la puntuación de exposición Administración de amenazas y vulnerabilidades la organización o la puntuación segura de Microsoft para dispositivos.
 
Si aún no quieres ver determinados dispositivos en la vista Inventario de dispositivos, intenta colocar una etiqueta de dispositivo para filtrar el dispositivo dado de baja de la vista Inventario de dispositivos.

Para obtener más información, vea:

[Dispositivos offboard del servicio Microsoft Defender para endpoints](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Puntuación de exposición en Administración de amenazas y vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Corregir sensores incorrectos en Microsoft Defender para endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cómo usar el etiquetado de forma eficaz (parte 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cómo usar el etiquetado de forma eficaz (parte 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cómo usar el etiquetado de forma eficaz (parte 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




