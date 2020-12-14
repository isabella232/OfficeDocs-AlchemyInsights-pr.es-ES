---
title: No se devolvieron resultados durante la búsqueda o exportación de contenido
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666666"
---
# <a name="no-results-returned-during-content-searchexport"></a>No se devolvieron resultados durante la búsqueda o exportación de contenido

Si experimenta problemas con los siguientes escenarios de exhibición de documentos electrónicos:

- La búsqueda y la exportación de contenido no devuelve datos o datos inesperados
- error de búsqueda o exportación de eDiscovery

Esto puede deberse a ciertos filtros de seguridad de cumplimiento que fueron configurados por un administrador específico y que no se han comunicado a todos los administradores.

Para solucionar esto, compruebe si hay filtros de seguridad de cumplimiento que puedan causar estos problemas:

1. Conectarse al centro de seguridad y cumplimiento PowerShell
2. Ejecute el siguiente commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obtener información adicional sobre los filtros de seguridad de cumplimiento, consulte [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
