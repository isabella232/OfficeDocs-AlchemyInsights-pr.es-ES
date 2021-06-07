---
title: Problemas de rendimiento en Microsoft Defender para punto de conexión en Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783444"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemas de rendimiento en Microsoft Defender para punto de conexión en Linux

Este artículo le mostrará los pasos para identificar problemas de rendimiento en Microsoft Defender para punto de conexión en Linux.

Es importante que primero compruebe si el problema que experimenta se ha resuelto en la[última versión](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Para iniciar su investigación, consulte cómo [Resolver problemas de rendimiento de Microsoft Defender para punto de conexión para Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Exclusiones

Las exclusiones pueden ayudar a mitigar los problemas de rendimiento. Revise las exclusiones antes de empezar para que se conozca y documente cualquier riesgo adicional.

Para más información, consulte [Configurar y validar exclusiones de Microsoft Defender para punto de conexión en Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

Si tiene varios archivos y carpetas a excluir y están todos en el mismo punto de montaje, puede ser más fácil excluir el punto de montaje. A partir de la versión 101.22.80 de febrero, se permite excluir un punto de montaje entero.

Por ejemplo, si /mnt/backup es un punto de montaje, puede agregar /mnt/backup a la lista de exclusión con este comando:

`$ mdatp exclusion folder add –path /mnt/backup`

**Nota**: Agregar exclusiones aumenta el riesgo de que no se detecte malware y debe administrarse e implementarse con cuidado.

## <a name="need-help"></a>¿Necesita ayuda?

Para ayudarle de la manera más eficaz, recopile los datos de diagnóstico antes de abrir un caso de soporte técnico.
