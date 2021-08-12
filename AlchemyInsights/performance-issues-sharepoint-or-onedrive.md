---
title: Problemas de rendimiento SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911859"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccesible o no disponible para varios usuarios

SharePoint o OneDrive pueden ser lentos, inaccesibles o no disponibles, o pueden mostrar errores de servicio no disponibles o 503, por varios motivos:
  
- Si el sitio SharePoint o OneDrive es lento o retrasa para varios usuarios, puede haber un problema de servicio temporal en el que los usuarios experimenten retrasos intermitentes o errores de navegación al acceder SharePoint sitios o OneDrive contenido. Consulte el [panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para comprobar si la organización está afectada.
  
- Es posible que los usuarios reciban un error *de 503* servidor ocupado al intentar navegar a SharePoint o OneDrive sitios. Este error puede deberse a la limitación dentro del SharePoint servicio. SharePoint Online utiliza limitación para mantener un rendimiento óptimo y la confiabilidad del servicio SharePoint Online. La limitación restringe el número de acciones de usuario o llamadas simultáneas (mediante script o código) para evitar el uso excesivo de recursos. Para obtener más información sobre la limitación, vea [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Si experimenta un rendimiento lento  con **una** página o un sitio SharePoint clásico o moderno, use la herramienta [diagnóstico](https://aka.ms/perftool) de página para analizar las páginas.
  
- Si sigue experimentando un rendimiento general lento, revise los recursos de la parte inferior de este artículo: Introducción a la optimización del rendimiento [para SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  