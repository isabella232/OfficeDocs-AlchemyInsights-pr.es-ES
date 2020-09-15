---
title: Herramienta de exportación de exhibición de documentos electrónicos
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711112"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>¿No puede instalar ni ejecutar la herramienta de exportación de exhibición de documentos electrónicos?

Si no puede instalar ni ejecutar la herramienta de exportación de exhibición de documentos electrónicos para descargar los resultados de la búsqueda, compruebe lo siguiente:
  
- El equipo que está usando cumple estos requisitos previos:

  - Versiones de 32 o 64 bits de Windows 7 y versiones posteriores

  - Microsoft .NET Framework 4.7

  - Un explorador compatible:

  - Microsoft Edge

    O bien:

  - Internet Explorer 10 y versiones posteriores

    No se admiten otros exploradores, como Google Chrome y Mozilla Firefox.

- Su organización puede conectarse al extremo en Azure, que es ** \* . BLOB.Core.Windows.net** (el carácter comodín representa un identificador único para su trabajo de exportación).

- Tiene asignada la función Export en el centro de seguridad y cumplimiento de Microsoft 365 &amp; . De forma predeterminada, este rol solo se asigna al grupo de roles eDiscovery Manager. Consulte [asignar permisos de exhibición](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)de documentos electrónicos.

Para obtener más información, vea [exportar resultados](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)de la búsqueda de contenido.
  