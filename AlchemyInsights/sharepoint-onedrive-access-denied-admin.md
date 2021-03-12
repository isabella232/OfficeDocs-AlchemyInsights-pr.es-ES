---
title: Solucionar problemas de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707971"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Solucionar problemas de acceso denegado de mensajes en El Centro de administración de Sharepoint/OneDrive

Si recibe un mensaje de acceso denegado al intentar navegar a un Centro de administración de Sharepoint/OneDrive, asegúrese de asignar una licencia [al usuario](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Si el usuario tiene una licencia, también debe asegurarse de que se les asigna un rol de [administrador](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) que pueda tener acceso a los centros de administración.

Este problema también puede producirse cuando un usuario se elimina y se vuelve a crear con el mismo nombre principal de usuario (UPN). La nueva cuenta se crea mediante un valor puid (identificador único de Passport) diferente. Cuando el usuario intenta obtener acceso a una colección de sitios o a su OneDrive, el usuario tiene un PUID incorrecto. Un segundo escenario implica la sincronización de directorios con una unidad organizativa (OU) de Active Directory. Si los usuarios ya han iniciado sesión en SharePoint y, a continuación, se mueven a otra unidad organizativa y se vuelve a sincronizar con SharePoint, pueden experimentar este problema.

Para resolver este problema, debe restaurar el UPN original con los pasos descritos en el artículo Restaurar [un usuario en Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: Si un Centro de administración de OneDrive o SharePoint no está disponible para varios usuarios que tenían acceso anteriormente, puede haber un problema de servicio temporal.  [Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).


