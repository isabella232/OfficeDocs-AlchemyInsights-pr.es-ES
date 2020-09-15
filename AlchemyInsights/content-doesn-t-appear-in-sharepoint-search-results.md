---
title: El contenido no aparece en los resultados de la búsqueda de SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713147"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>El contenido no aparece en los resultados de la búsqueda de SharePoint

Siga estos pasos de solución de problemas cuando el contenido esperado no aparece en los resultados de búsqueda:
  
1. Compruebe que el **sitio** que contiene el contenido esperado está configurado para permitir que el contenido aparezca en los resultados de búsqueda. Siga los pasos descritos en [Mostrar contenido en un sitio de los resultados de búsqueda](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Compruebe que la **lista** o **biblioteca** que contiene el contenido esperado esté configurada para permitir que el contenido aparezca en los resultados de búsqueda. Siga los pasos que se indican en [Mostrar contenido de listas o bibliotecas en los resultados de búsqueda](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Compruebe que la página, el documento o el diseño de página personalizado está publicado como una **versión principal.** Seguir el paso 3 de la [búsqueda no devuelve todos los resultados en SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Compruebe que el usuario tiene **permisos** para ver el contenido. Siga los pasos descritos en Understanding [Levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Si se ha cambiado el esquema de búsqueda mediante la adición de una nueva propiedad administrada, mediante la edición de una propiedad administrada o mediante la eliminación de una propiedad administrada, será necesario solicitar un rastreo y volver a indizar. Para **volver a indizar** el contenido, siga los pasos descritos en [solicitar manualmente el rastreo y la reindización de un sitio, una biblioteca o una lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Esto puede tardar un rato, esperar 24 horas antes de volver a revisar los resultados.

Para obtener más información, vea [Habilitar el contenido de un sitio para que se pueda buscar](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
