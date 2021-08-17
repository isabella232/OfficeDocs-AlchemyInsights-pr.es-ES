---
title: El contenido no aparece en los SharePoint de búsqueda
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081627"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>El contenido no aparece en los SharePoint de búsqueda

Siga estos pasos de solución de problemas cuando el contenido esperado no aparezca en los resultados de la búsqueda:
  
1. Compruebe que el **sitio que** contiene el contenido esperado está configurado para permitir que el contenido aparezca en los resultados de búsqueda. Siga los pasos descritos en [Mostrar contenido en un sitio en los resultados de búsqueda.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Compruebe que la **lista o** **biblioteca** que contiene el contenido esperado esté establecida para permitir que el contenido aparezca en los resultados de la búsqueda. Siga los pasos descritos en [Mostrar contenido de listas o bibliotecas en los resultados de búsqueda.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Compruebe que el diseño de página, documento o página personalizado se publique como **versión principal.** Siga el paso 3 en La búsqueda no devuelve todos los [resultados en SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Compruebe que el usuario tiene **permisos para** ver el contenido. Siga los pasos descritos en [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Si el esquema de búsqueda se ha cambiado agregando una nueva propiedad administrada, editando una propiedad administrada o quitando una propiedad administrada, será necesario solicitar un rastreo y un nuevo índice. **Vuelva a indizar** el contenido siguiendo los pasos descritos en Solicitar manualmente el rastreo y [la nueva indización](https://docs.microsoft.com/sharepoint/crawl-site-content)de un sitio, una biblioteca o una lista . Esto puede tardar un tiempo, espere 24 horas antes de volver a comprobar los resultados.

Para obtener más información, vea [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
