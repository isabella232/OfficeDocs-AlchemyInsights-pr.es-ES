---
title: Solución de problemas de acceso denegado de mensajes OneDrive para la Empresa sitios
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957810"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Solución de problemas de acceso denegado de mensajes OneDrive para la Empresa sitios

Este problema se produce con más frecuencia cuando un usuario se elimina y se vuelve a crear con el mismo nombre principal de usuario (UPN). La nueva cuenta se crea mediante un valor puid (identificador único de Passport) diferente. Cuando el usuario intenta obtener acceso a una colección de sitios o a su OneDrive, el usuario tiene un PUID incorrecto. Un segundo escenario implica la sincronización de directorios con una unidad organizativa (OU) de Active Directory. Si los usuarios ya han iniciado sesión en SharePoint y, a continuación, se mueven a una UO diferente y se vuelve a sincronizar con SharePoint, pueden experimentar este problema.

1. Para resolver este problema, debe restaurar el UPN original con los pasos del artículo, [Restaurar un usuario en Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Si no puede restaurar el usuario original, debe quitar el usuario antiguo del sitio OneDrive mediante estos pasos, Quite un usuario de la lista de información [de usuario](). 
3. Una vez hecho esto, puede comprobar que el usuario tiene derechos de administrador en el sitio de OneDrive siguiendo los pasos para Agregar administradores para el sitio de [un usuario](https://docs.microsoft.com/sharepoint/manage-user-profiles) OneDrive

Para obtener más información sobre los niveles de permisos, vea el artículo Descripción de los niveles de [permisos en SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
