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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058019"
---
# <a name="no-results-from-content-searchexports"></a>Sin resultados de búsqueda o exportación de contenido

Los problemas con la búsqueda o las exportaciones de contenido que no devuelven datos pueden deberse a cierto filtro de seguridad de cumplimiento configurado por un administrador específico y a no comunicarlo a todos los administradores.

Para resolver esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando esto:
1. Conectar a Powershell del Centro de seguridad y cumplimiento
2. Ejecute los siguientes comandos:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org