---
title: Pausar actualizaciones programadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530597"
---
# <a name="pausing-scheduled-updates"></a>Pausar actualizaciones programadas

Cuando se ejecuta un comando pause, los dispositivos no procesan el comando hasta la próxima vez que se registran en Intune. Por este motivo, es posible que los dispositivos:

- Tengan instaladas las actualizaciones programadas antes del registro.
- Se hayan apagado cuando se emitió el comando pause. En este caso, cuando se enciendan los dispositivos, es posible que se hayan descargado e instalado las actualizaciones programadas anteriores al registro.