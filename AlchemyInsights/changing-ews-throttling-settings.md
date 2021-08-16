---
title: Cambiar la de velocidad moderada de EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968394"
---
# <a name="changing-ews-throttling-settings"></a>Cambiar la de velocidad moderada de EWS

Ejecute la prueba automatizada, que le permitirá modificar la directiva de velocidad moderada de EWS durante la migración. Tenga en cuenta que, incluso después de que se ejecute, las importaciones EWS seguirán estando limitadas a 150 mb por 5 minutos por buzón; para alcanzar una mayor velocidad de rendimiento de la migración, migre más usuarios a la vez.

Tenga en cuenta que los cambios en la Directiva de limitación de EWS no tienen efecto en los siguientes tipos de migración (con las herramientas de Microsoft): híbrida, total/preconfigurada (RPC/HTTP), IMAP, G Suite, carpeta pública o servicio de importación de PST.