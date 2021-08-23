---
title: Alertas que faltan en la pestaña Alertas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362415"
---
# <a name="alerts-missing-from-alerts-tab"></a>Alertas que faltan en la pestaña Alertas

La **pestaña Alertas** funciona en función de las directivas de configuración y activadas del portal de gobierno de aplicaciones del inquilino. También se deben activar las directivas personalizadas en App Governance para permitir que las señales fluyan a la **pestaña Alertas.** 

Confirme que se ha generado la alerta:

1. Ve a Directivas de gobierno [de](https://compliance.microsoft.com/m365appprotection?viewid=policies) aplicaciones y confirma que has creado al menos una directiva de auditoría o activa.

1. Seleccione la directiva y, a continuación, seleect **Edit** en el panel desplegable. 

1. Compruebe la configuración de la directiva para confirmar que se debería haber generado una alerta en función de un evento de directiva iniciado hace más de 24 horas.

Para obtener más información sobre las alertas en App Governance, consulta Introducción a la detección y corrección de amenazas [de aplicaciones.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)