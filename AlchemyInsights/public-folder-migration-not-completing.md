---
title: El lote de migración de la carpeta pública no completado, se muestra sincronizado.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406610"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>El lote de migración de la carpeta pública no completado, se muestra sincronizado.

Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando “Sincronizado” por mucho tiempo. Este es el comportamiento esperado.

Es habitual que el estado del lote de migración permanezca como Sincronizado durante algunas horas, antes de que cambie a Completando. En el caso de las migraciones que impliquen un número grande de buzones objetivo, es normal que el estado permanezca en estado Sincronizado por más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de la carpeta pública subyacente haya fallado ni esté en cuarentena. Permita un lapso de 24 a 48 horas para que el lote de migración finalice las tareas.
