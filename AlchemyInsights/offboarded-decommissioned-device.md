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
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324461"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemas con la eliminación de un dispositivo fuera deborde o retirada del inventario de dispositivos

Actualmente, Microsoft Defender para endpoint no permite quitar manualmente el registro de dispositivo de un dispositivo fuera deborde o dado de baja del Inventario de dispositivos.

Por motivos de seguridad, el dispositivo permanece en el portal como un registro histórico hasta 180 días. Sin embargo, los datos del dispositivo se purgan según el período de retención configurado.

**Nota:** Un dispositivo fuera deborde o desmantelado cambia automáticamente al **estado inactivo** después de siete días. Además, los dispositivos que no están activos en los últimos 30 días no se tienen en cuenta en los datos que reflejan la puntuación de exposición Administración de amenazas y vulnerabilidades la organización o la puntuación segura de Microsoft para dispositivos.
 
Si aún no quieres ver determinados dispositivos en la vista Inventario de dispositivos, intenta colocar una etiqueta de dispositivo para filtrar el dispositivo dado de baja de la vista Inventario de dispositivos.

Para más información, consulte:

[Dispositivos offboard del servicio Microsoft Defender para endpoints](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Puntuación de exposición en Administración de amenazas y vulnerabilidades](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Corregir sensores incorrectos en Microsoft Defender para endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cómo usar el etiquetado de forma eficaz (parte 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cómo usar el etiquetado de forma eficaz (parte 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cómo usar el etiquetado de forma eficaz (parte 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




