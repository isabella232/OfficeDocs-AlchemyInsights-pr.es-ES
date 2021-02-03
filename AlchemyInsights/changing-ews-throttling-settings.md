---
title: Cambiar la de velocidad moderada de EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075914"
---
# <a name="changing-ews-throttling-settings"></a>Cambiar la de velocidad moderada de EWS

Ejecute la prueba automatizada, que le permitirá modificar la directiva de velocidad moderada de EWS durante la migración. Tenga en cuenta que, incluso después de que se ejecute, las importaciones EWS seguirán estando limitadas a 150 mb por 5 minutos por buzón; para alcanzar una mayor velocidad de rendimiento de la migración, migre más usuarios a la vez.

Tenga en cuenta que los cambios en la Directiva de limitación de EWS no tienen efecto en los siguientes tipos de migración (con las herramientas de Microsoft): híbrida, total/preconfigurada (RPC/HTTP), IMAP, G Suite, carpeta pública o servicio de importación de PST.