---
title: Problemas con la incorporación de equipos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139058"
---
# <a name="issues-with-onboarding-machines"></a>Problemas con la incorporación de equipos

Es posible que tenga problemas con la incorporación de equipos al servicio de MDATP. Si puede obtener acceso al equipo del usuario final, siga estos pasos:

1. Descargue la herramienta de diagnóstico [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).
2. Extraiga y ejecute MDATPAnalyzer.cmd.
3. Busque el registro de diagnóstico en la carpeta llamada MDATPClientAnalyzerResult, la misma carpeta en la que se ha descargado la herramienta de diagnóstico.
4. Revise el archivo de registro, MDATPClientAnalyzer.txt, para buscar problemas de configuración del proxy de Internet o de conectividad.