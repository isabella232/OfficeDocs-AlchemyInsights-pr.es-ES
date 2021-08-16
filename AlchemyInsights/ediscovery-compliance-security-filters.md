---
title: No se devuelven resultados durante la búsqueda o exportación de contenido
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101283"
---
# <a name="no-results-returned-during-content-searchexport"></a>No se devuelven resultados durante la búsqueda o exportación de contenido

Si tiene problemas con los siguientes escenarios de exhibición de documentos electrónicos:

- Búsqueda/exportación de contenido no devuelve datos ni datos inesperados
- Error en la búsqueda o exportación de exhibición de documentos electrónicos

Esto puede deberse a ciertos filtros de seguridad de cumplimiento configurados por un administrador específico y que no se han comunicado a todos los administradores.

Para resolver esto, compruebe si hay filtros de seguridad de cumplimiento que puedan estar causando estos problemas:

1. Conectar a Powershell del Centro de seguridad y cumplimiento
2. Ejecute los siguientes comandos:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Para obtener información adicional sobre los filtros de seguridad de cumplimiento, [vea Filtrado de permisos para la búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
