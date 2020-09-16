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
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771738"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Eliminar permanentemente un sitio de SharePoint

Para volver a usar una dirección URL de un sitio eliminado (para volver a crear un sitio) o para eliminar permanentemente un sitio porque ya no está en uso, puede usar **Eliminar permanentemente** del nuevo Centro de administración de SharePoint. 

1. Vaya a la página [Sitios eliminados del nuevo Centro de administración de SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e inicie sesión con una cuenta que tenga permisos de administrador para su organización. 

2. En la columna de la izquierda, seleccione un sitio. 

3. Haga clic en **Eliminar permanentemente** 

**Tenga en cuenta**: los sitios conectados a un grupo no se pueden eliminar permanentemente desde el nuevo Centro de administración de SharePoint. Se debe usar [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) en su lugar.  

Para obtener más información, vea [Eliminar de forma permanente un sitio](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
