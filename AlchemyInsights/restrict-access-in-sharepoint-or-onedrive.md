---
title: Restringir el acceso en SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075057"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Restringir el acceso en SharePoint o OneDrive

En SharePoint y OneDrive, se restringe el acceso a elementos como archivos, carpetas y listas mediante la concesión de acceso solo a grupos o personas a las que desea tener acceso. De forma predeterminada, los permisos SharePoint se heredan de una parte superior de la jerarquía. Por lo tanto, un archivo hereda sus permisos de la carpeta, que hereda sus permisos de la biblioteca, que hereda sus permisos del sitio.
  
Puede compartir en un nivel superior (por ejemplo, mediante el uso compartido de un sitio completo) y, a continuación, interrumpir la herencia si no desea compartir todos los elementos del sitio. Sin embargo, no se recomienda esto porque hace que mantener los permisos sea más complejo y confuso en el futuro. Esto es lo que podrías hacer en su lugar:
  
- Si, por ejemplo, desea compartir todo el contenido de una carpeta excepto un archivo en ella, mueva ese archivo a una nueva ubicación que no esté compartida.
    
- Si tiene dos subcarpetas en una carpeta y desea compartir una subcarpeta con los grupos A y B y permitir solo el acceso del grupo A a la segunda subcarpeta, comparta la carpeta principal con el grupo A y agregue el grupo B a la primera subcarpeta.
    
[Dejar de compartir un archivo o carpeta ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

