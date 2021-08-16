---
title: Sitio moderno como sitio raíz
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000409"
---
# <a name="modern-site-as-root-site"></a>Sitio moderno como sitio raíz

We have started to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site). Use [Invoke-SPOSiteSwap para](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) intercambiar la ubicación de un sitio con otro sitio mientras se archiva el sitio original. Disponible tanto para el sitio de grupo (no conectado a un grupo) como para el sitio de comunicación.

>[!Important]
> No elimine el sitio raíz clásico para crear un sitio de comunicación moderno. Microsoft no admite esta opción. Al eliminar el sitio raíz, todos los sitios SharePoint de la organización serán inaccesibles para todos los usuarios, hasta que restaure el sitio o cree un nuevo sitio en la misma dirección URL. Comunicaremos esta característica a través del centro de mensajes. Debe esperar que la característica se encenda en el espacio empresarial en breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conocidos con el intercambio de sitios
- El sitio de destino puede devolver un error "no encontrado" (HTTP 404) durante un breve período de tiempo.
- El contenido tendrá que volver a buscarse para actualizar el índice de búsqueda. No hay ningún paso manual necesario aquí, esto se realizará automáticamente.
- Cualquier cosa que dependa de vínculos "estáticos" (como La sincronización de archivos y OneNote archivos) tendrá que corregirse manualmente.
- Project Es posible que los sitios de servidor deba validarse para asegurarse de que siguen estando asociados correctamente. 
