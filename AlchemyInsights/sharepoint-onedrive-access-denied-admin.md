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
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085245"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Solucionar problemas de acceso denegado mensajes en Sharepoint/OneDrive Admin Center

Si recibe un mensaje de acceso denegado al intentar navegar a un Centro de administración de Sharepoint/OneDrive, asegúrese de asignar una licencia [al usuario](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Si el usuario tiene una licencia, también debe asegurarse de que se les asigna un rol de [administrador](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) que pueda tener acceso a los centros de administración.

Este problema también puede producirse cuando un usuario se elimina y se vuelve a crear con el mismo nombre principal de usuario (UPN). La nueva cuenta se crea mediante un valor puid (identificador único de Passport) diferente. Cuando el usuario intenta obtener acceso a una colección de sitios o a su OneDrive, el usuario tiene un PUID incorrecto. Un segundo escenario implica la sincronización de directorios con una unidad organizativa (OU) de Active Directory. Si los usuarios ya han iniciado sesión en SharePoint y, a continuación, se mueven a una UO diferente y se vuelve a sincronizar con SharePoint, pueden experimentar este problema.

Para resolver este problema, debe restaurar el UPN original con los pasos del artículo Restaurar un usuario [en Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Nota: Si un centro OneDrive o SharePoint de administración no está disponible para varios usuarios que tenían acceso anteriormente, puede haber un problema de servicio temporal.  [Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).


