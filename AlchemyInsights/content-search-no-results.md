---
title: Búsqueda de contenido sin resultados
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816865"
---
# <a name="no-results-from-content-searchexports"></a>Sin resultados de búsqueda o exportación de contenido

Los problemas con la búsqueda o las exportaciones de contenido que no devuelven datos pueden deberse a cierto filtro de seguridad de cumplimiento configurado por un administrador específico y a no comunicarlo a todos los administradores.

Para resolver esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando esto:
1. Conectarse a PowerShell del Centro de seguridad y cumplimiento
2. Ejecute los siguientes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org