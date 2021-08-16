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
ms.openlocfilehash: 7ea6c56de00a52080c4a8b47eb5eeee37838420a9e979878c10aeb12885a8b99
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010506"
---
# <a name="pausing-scheduled-updates"></a>Pausar actualizaciones programadas

Cuando se ejecuta un comando Pausa, los dispositivos no procesan el comando hasta la próxima vez que se registran en Intune. Debido a esto, sus dispositivos pueden tener:

- Instaladas las actualizaciones programadas antes del registro.
- Desactivadas cuando utilizó el comando Pausa. En este caso, cuando se encendieron los dispositivos, es posible que se hayan descargado e instalado las actualizaciones programadas anteriores al registro.