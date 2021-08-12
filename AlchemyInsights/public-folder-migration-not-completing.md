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
ms.openlocfilehash: 1c768dcc79d39ac4164a86f7f82bd6be490cdc4df48a11d2f198fece492eba38
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911211"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a>El lote de migración de la carpeta pública no completado, se muestra sincronizado.

Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando “Sincronizado” por mucho tiempo. Este es el comportamiento que se espera.

Es habitual que el estado del lote de migración permanezca como Sincronizado durante algunas horas, antes de que cambie a Completando. En el caso de las migraciones que impliquen un número grande de buzones objetivo, es normal que el estado permanezca en estado Sincronizado por más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de la carpeta pública subyacente haya fallado ni esté en cuarentena. Permita un lapso de 24 a 48 horas para que el lote de migración finalice las tareas.
