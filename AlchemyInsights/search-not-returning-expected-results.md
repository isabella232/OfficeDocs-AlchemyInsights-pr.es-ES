---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052727"
---
# <a name="content-search-not-returning-expected-results"></a>Búsqueda de contenido no devuelve los resultados esperados

Al ejecutar búsquedas de contenido desde el centro Microsoft 365 seguridad & cumplimiento, es posible que reciba resultados de búsqueda inesperados. Tenga en cuenta lo siguiente que puede afectar a los resultados de la búsqueda:

- **Ubicaciones de contenido y condiciones de búsqueda:** asegúrese de que ha seleccionado las ubicaciones de contenido y las condiciones de búsqueda adecuadas. Si ha ejecutado una búsqueda de gran tamaño (con muchas ubicaciones), considere la posibilidad de dividirla en varias búsquedas.

- **Elementos parcialmente indizados:** los elementos  [parcialmente indizados](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) de los buzones se incluyen en los resultados de búsqueda estimados. Sin embargo, los elementos parcialmente indizados de los sitios de SharePoint y OneDrive no se incluyen en la estimación de búsqueda.

- Errores de búsqueda: al buscar un gran número de buzones (más de 100 000 **buzones),** puede obtener errores de búsqueda, con códigos de error como CS008-009 y CS012-002). En este caso, reintente la búsqueda solo para las ubicaciones de contenido con errores. Vea  [este artículo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obtener más información.
