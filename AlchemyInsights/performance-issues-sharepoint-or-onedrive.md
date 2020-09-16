---
title: 'Problemas de rendimiento: SharePoint o OneDrive'
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771918"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive es lento, inaccesible o no disponible para varios usuarios

SharePoint o OneDrive puede ser lento, inaccesible o no disponible, o puede mostrar los errores servicio no disponible o 503, por varios motivos:
  
- Si el sitio de SharePoint o de OneDrive es lento o se retrasa para varios usuarios, es posible que haya un problema de servicio temporal en el que los usuarios experimenten retrasos intermitentes o errores de navegación al obtener acceso a sitios de SharePoint o contenido de OneDrive. Consulte el [panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para comprobar si la organización está afectada.
  
- Es posible que los usuarios reciban un error de un *servidor de 503* al intentar navegar a sitios de SharePoint o de OneDrive. Este error puede deberse a una limitación en el servicio de SharePoint. SharePoint Online utiliza limitación para mantener un rendimiento óptimo y la confiabilidad del servicio SharePoint Online. La limitación restringe el número de acciones de usuario o llamadas simultáneas (mediante script o código) para evitar el uso excesivo de recursos. Para obtener más información sobre la limitación de peticiones, consulte [limitar o bloqueado en SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Si experimenta un rendimiento lento con un sitio o página de SharePoint **clásico** o **moderno** , use la [herramienta de diagnóstico de páginas](https://aka.ms/perftool) para analizar las páginas.
  
- Si sigue experimentando un rendimiento lento general, revise los recursos que se encuentra en la parte inferior de este artículo: [Introducción al ajuste del rendimiento de SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334) .
  