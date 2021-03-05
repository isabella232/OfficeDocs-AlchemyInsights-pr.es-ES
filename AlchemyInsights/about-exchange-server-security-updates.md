---
title: Acerca Exchange Server actualizaciones de seguridad
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449157"
---
# <a name="about-exchange-server-security-updates"></a>Acerca Exchange Server actualizaciones de seguridad

Microsoft ha publicado una serie de actualizaciones de seguridad críticas Exchange Server locales. Las versiones de servidor afectadas son los niveles de actualización de Exchange Server 2010, 2013, 2016 y 2019. Exchange Online NO se ve afectado, pero si tiene algunos servidores de Exchange locales debido a la configuración híbrida, son potencialmente vulnerables.

Para actualizar los servidores locales, tendrá que ejecutar al menos las siguientes versiones de Exchange:

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 o CU 18
- Exchange Server 2019 CU 8 o CU 7

Consulte el siguiente anuncio para ver la ubicación de las [correcciones: Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Notas importantes:**

La instalación de actualizaciones no funcionará si los servidores locales no ejecutan las versiones de Exchange necesarias, según la lista anterior.

Si instala actualizaciones manualmente, lea la sección "Problemas conocidos" de los artículos de KB de actualización para obtener información importante. Las actualizaciones de seguridad DEBEN ejecutarse desde un símbolo del sistema de CMD/PowerShell con privilegios elevados.
