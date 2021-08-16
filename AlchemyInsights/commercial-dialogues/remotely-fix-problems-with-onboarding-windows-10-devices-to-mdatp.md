---
title: Solucionar problemas de forma remota con la incorporación de Windows 10 dispositivos a la Protección contra amenazas avanzada de Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034051"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Solucionar problemas de forma remota con la incorporación de Windows 10 dispositivos a la Protección contra amenazas avanzada de Microsoft Defender

Si puede tener acceso al equipo remoto, siga estos pasos:

1. Descargue la herramienta de diagnóstico [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Extraiga y ejecute MDATPAnalyzer.cmd.
3. Busque el registro de diagnóstico en la carpeta MDATPClientAnalyzerResult, que es la misma carpeta donde se descargó la herramienta Analizador.
4. Para encontrar problemas con la configuración de proxy de Internet o conectividad, revise el archivo de registro MDATPClientAnalyzer.txt.

Para obtener más información, vea [Problemas con las máquinas de incorporación.](https://go.microsoft.com/fwlink/?linkid=2143634)
