---
title: 1490-solución de problemas-errores de exhibición de documentos electrónicos
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277818"
---
# <a name="troubleshoot-content-search-errors"></a>Solucionar errores de búsqueda de contenido

¿Tiene problemas con la búsqueda de contenido o la obtención de errores al exportar los resultados de la búsqueda?

Por ejemplo, ¿recibe lo siguiente cuando ejecuta búsquedas?

- Errores CS008 o CS012

- Errores de tiempo de espera o de servidor ocupado

- Se produjo un error en la aplicación

O bien, al buscar o exportar resultados de un gran número de buzones (más de 100.000 buzones), ¿recibe errores de exportación?

Para estos tipos de errores, vuelva a intentar la búsqueda de las ubicaciones de contenido que han fallado. Consulte  [este artículo](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) para obtener más información.

Si va a exportar más de 100 k buzones, tendrá que usar el siguiente PowerShell para descargar los resultados de la exportación:  [exportar resultados de más de 100 k buzones de correo](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
