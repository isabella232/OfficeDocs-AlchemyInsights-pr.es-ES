---
title: Pausar actualizaciones programadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721572"
---
# <a name="pausing-scheduled-updates"></a>Pausar actualizaciones programadas

Cuando se ejecuta un comando pause, los dispositivos no procesan el comando hasta la próxima vez que se registran en Intune. Por este motivo, es posible que los dispositivos:

- Tengan instaladas las actualizaciones programadas antes del registro.
- Se hayan apagado cuando se emitió el comando pause. En este caso, cuando se enciendan los dispositivos, es posible que se hayan descargado e instalado las actualizaciones programadas anteriores al registro.