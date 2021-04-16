---
title: Herramienta de exportación de exhibición de documentos electrónicos
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814605"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>¿No se puede instalar o ejecutar la herramienta de exportación de exhibición de documentos electrónicos?

Si no puede instalar o ejecutar la herramienta de exportación de exhibición de documentos electrónicos para descargar los resultados de búsqueda, compruebe lo siguiente:
  
- El equipo que está usando cumple estos requisitos previos:

  - Versiones de 32 o 64 bits de Windows 7 y versiones posteriores

  - Microsoft .NET Framework 4.7

  - Un explorador compatible:

  - Microsoft Edge

    O bien:

  - Internet Explorer 10 y versiones posteriores

    No se admiten otros exploradores, como Google Chrome y Mozilla Firefox.

- Su organización puede conectarse al punto de conexión de Azure, que **\* es .blob.core.windows.net** (el comodín representa un identificador único para el trabajo de exportación).

- Se le asigna el rol Exportar en el Centro de cumplimiento de seguridad de Microsoft 365. &amp; De forma predeterminada, este rol solo se asigna al grupo de roles administrador de exhibición de documentos electrónicos. Vea [Asignar permisos de exhibición de documentos electrónicos.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Para obtener más información, vea [Exportar resultados de búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Si exporta más de 100.000 buzones, deberá usar el siguiente Powershell para descargar los resultados de exportación: Exportar resultados de más de [100 mil buzones.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)