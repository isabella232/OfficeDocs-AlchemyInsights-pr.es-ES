---
title: Intercambiar el sitio raíz clásico con un sitio moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316157"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Intercambiar el sitio raíz clásico con un sitio moderno

Si el entorno se ha configurado antes de abril de 2019, puede cambiar el sitio raíz a un sitio moderno mediante Microsoft PowerShell:

- Si tiene un sitio diferente que desea usar como sitio raíz, puede reemplazar [(intercambiar) el sitio raíz](https://docs.microsoft.com/sharepoint/modern-root-site) por él. 
    - Use [Invoke-SPOSiteSwap para](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) intercambiar la ubicación de un sitio con otro sitio mientras se archiva el sitio original. Disponible tanto para el sitio de grupo (no conectado a un grupo) como para el sitio de comunicación. 

- Próximamente se introducirán funciones adicionales que le permitirán seguir usando el contenido del sitio, pero convertir el sitio existente en un sitio de comunicación. 

**Importante:** Estas funcionalidades se van a implantar gradualmente. Continúe buscando actualizaciones en el Centro de mensajes. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conocidos con el intercambio de sitios

- El sitio de destino puede devolver un error "no encontrado" (HTTP 404) durante un breve período de tiempo.
- El contenido tendrá que volver a buscarse para actualizar el índice de búsqueda. No es necesario realizar ningún paso manual: esto se realizará automáticamente.
- Cualquier cosa que dependa de vínculos "estáticos" (como La sincronización de archivos y OneNote archivos) tendrá que corregirse manualmente.
- Si el sitio de origen era un sitio de noticias de la organización, actualice la dirección URL. Obtener una lista de todos los sitios de noticias de la organización.
- Project Es posible que los sitios de servidor deba validarse para asegurarse de que siguen estando asociados correctamente.
