---
title: Jubilación de servicios de Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698699"
---
# <a name="access-services-retirement"></a>Jubilación de servicios de Access

Como se anunció originalmente en MC97576, en el 2017 de marzo, y se siguió comunicándose a través del último año, los servicios de Access se están retirando. La siguiente fase de este proceso será la eliminación de las bases de datos Web de Access que usan listas de SharePoint como almacenamiento de datos subyacente.

**¿Qué me afecta?**

A partir del 2019 de junio, deteneremos la creación de nuevas bases de datos de Access en SharePoint Online y cerrará el servicio y el resto de las aplicaciones hasta el 2020 de abril.

**¿Qué debo hacer para prepararse para este cambio?**

Le recomendamos que cree un plan de transición para las bases de datos Web de Access de su organización. Los administradores pueden usar el [Explorador de aplicaciones de Access para SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obtener un inventario de las aplicaciones de Access que usan los sitios.

Hay varias formas de migrar los datos de bases de datos Web de Access:

- Importación a una base de datos de Access local (. ACCDB) o a un archivo de Excel.
- También se recomienda explorar Microsoft PowerApps como una plataforma alternativa para crear soluciones empresariales sin código para dispositivos móviles y Web.