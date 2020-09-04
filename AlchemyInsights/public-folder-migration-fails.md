---
title: Error en la migración de carpetas públicas al 95%
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
ms.openlocfilehash: c1c4210baf93f0071a12f1902fb5f6fbf7bd0716
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341389"
---
# <a name="public-folder-migration-fails-at-95"></a>Error en la migración de carpetas públicas al 95%

Es posible que haya iniciado la finalización de un lote de migración y que el estado del lote de migración siga mostrando **Sincronizado** durante un tiempo largo. Este es el comportamiento que se espera.

Es habitual que el estado de un lote de migración permanezca como **Sincronizado** durante unas horas antes de que cambie a **Completando**. En el caso de las migraciones que impliquen un gran número de buzones de destino, es normal que el estado permanezca en estado sincronizado durante más de 24 horas, siempre y cuando ninguna de las solicitudes de migración de carpeta pública subyacente falle o se ponga en cuarentena. Deje que el lote de migración finalice las 24/48 horas para completar las tareas.

En caso de que falle la migración de carpetas públicas al 95 %, con el error FailedToMailEnablePublicFoldersException:

1. Descargue y ejecute el script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) en el servidor local de Exchange.

2. Ejecute las acciones correctivas que sugiere el script.

3. Ejecute la sincronización-MailPublicFolders (para Exchange 2010) o Sync-ModernMailPublicFolders (para Exchange 2013 y versiones posteriores).

4. Reanude la migración de carpetas públicas.
