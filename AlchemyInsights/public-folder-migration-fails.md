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
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903620"
---
# <a name="public-folder-migration-fails-at-95"></a>Error en la migración de carpetas públicas al 95%

En caso de que falle la migración de carpetas públicas al 95%, con el error FailedToMailEnablePublicFoldersException:

1. Descargue y ejecute el script [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) en el servidor local de Exchange.

2. Ejecute las acciones correctivas que sugiere el script.

3. Ejecute la sincronización-MailPublicFolders (para Exchange 2010) o Sync-ModernMailPublicFolders (para Exchange 2013 y versiones posteriores).

4. Reanude la migración de carpetas públicas.
