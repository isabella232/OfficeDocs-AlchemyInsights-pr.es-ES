---
title: No hay resultados en la búsqueda de contenido
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680664"
---
# <a name="no-results-from-content-searchexports"></a>No hay resultados en la búsqueda/exportación de contenido

Problemas con la búsqueda y las exportaciones de contenido que no devuelven datos puede deberse a ciertos filtros de seguridad de cumplimiento que han sido configurados por un administrador específico y no lo comunican a todos los administradores.

Para solucionar esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando esto:
1. Conectarse al centro de seguridad y cumplimiento PowerShell
2. Ejecute el siguiente commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org