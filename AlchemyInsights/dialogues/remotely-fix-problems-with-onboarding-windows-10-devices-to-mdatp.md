---
title: Solucionar problemas de forma remota con la incorporación de dispositivos Windows 10 a la Protección contra amenazas avanzada de Microsoft Defender
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530133"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Solucionar problemas de forma remota con la incorporación de dispositivos Windows 10 a la Protección contra amenazas avanzada de Microsoft Defender

Si puede tener acceso al equipo remoto, siga estos pasos:

1. Descargue la herramienta de diagnóstico [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466).
2. Extraiga y ejecute MDATPAnalyzer.cmd.
3. Busque el registro de diagnóstico en la carpeta MDATPClientAnalyzerResult, que es la misma carpeta donde se descargó la herramienta Analizador.
4. Para encontrar problemas con la configuración de proxy de Internet o conectividad, revise el archivo de registro MDATPClientAnalyzer.txt.

Para obtener más información, vea [Problemas con las máquinas de incorporación.](https://go.microsoft.com/fwlink/?linkid=2143634)
