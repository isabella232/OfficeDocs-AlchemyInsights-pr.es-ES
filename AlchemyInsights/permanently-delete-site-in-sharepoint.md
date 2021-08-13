---
title: Eliminar permanentemente un sitio de SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944328"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Eliminar permanentemente un sitio de SharePoint

Para volver a usar una dirección URL de un sitio eliminado (para volver a crear un sitio) o para eliminar permanentemente un sitio porque ya no está en uso, puede usar **Eliminar permanentemente** del nuevo Centro de administración de SharePoint. 

1. Vaya a la página [Sitios eliminados del nuevo Centro de administración de SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e inicie sesión con una cuenta que tenga permisos de administrador para su organización. 

2. En la columna de la izquierda, seleccione un sitio. 

3. Haga clic en **Eliminar permanentemente** 

**Tenga en cuenta**: los sitios conectados a un grupo no se pueden eliminar permanentemente desde el nuevo Centro de administración de SharePoint. Se debe usar [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) en su lugar.  

Para obtener más información, vea [Eliminar de forma permanente un sitio](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
