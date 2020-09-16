---
title: El lote de migración de la carpeta pública no completado, se muestra sincronizado.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771491"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>El lote de migración de la carpeta pública no completado, se muestra sincronizado.

Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando “Sincronizado” por mucho tiempo. Este es el comportamiento esperado.

Es habitual que el estado del lote de migración permanezca como Sincronizado durante algunas horas, antes de que cambie a Completando. En el caso de las migraciones que impliquen un número grande de buzones objetivo, es normal que el estado permanezca en estado Sincronizado por más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de la carpeta pública subyacente haya fallado ni esté en cuarentena. Permita un lapso de 24 a 48 horas para que el lote de migración finalice las tareas.
