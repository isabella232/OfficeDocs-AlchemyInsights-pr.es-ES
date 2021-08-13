---
title: Retiro de servicios de access
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938712"
---
# <a name="access-services-retirement"></a>Retiro de servicios de access

Como anunciamos originalmente en MC97576, en marzo de 2017, y continuamos comunicándonos durante el año Access Services se están retirando. La siguiente fase de este proceso será la eliminación de bases de datos web de Access que usan listas SharePoint como almacenamiento de datos subyacente.

**¿Cómo me afecta esto?**

A partir de junio de 2019, detendrá la creación de nuevas bases de datos de Access en SharePoint Online y cerraremos el servicio y las aplicaciones restantes para abril de 2020.

**¿Qué debo hacer para prepararme para este cambio?**

Le recomendamos que cree un plan de transición para las bases de datos web de Access de su organización. Los administradores pueden usar [el SharePoint de aplicaciones de Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) para obtener un inventario de las aplicaciones de Access que usan los sitios.

Hay varias formas de migrar datos de bases de datos web de Access:

- Importación a una base de datos de Access local (. ACCDB) o a un Excel archivo.
- También recomendamos explorar Microsoft PowerApps como una plataforma alternativa para crear soluciones empresariales sin código para dispositivos móviles y web.