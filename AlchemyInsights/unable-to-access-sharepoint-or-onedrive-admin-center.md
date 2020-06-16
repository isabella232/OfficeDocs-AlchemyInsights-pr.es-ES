---
title: No se puede acceder al centro de administración de SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 627a4ef2900a6b9bbef7eb3f3a214ee7c371e354
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716472"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>No se puede acceder al centro de administración de SharePoint o OneDrive

- Si el sitio del centro de administración de SharePoint o OneDrive no es accesible o no está disponible, es posible que haya un problema de servicio temporal por el que los usuarios experimenten retrasos intermitentes o errores de navegación al acceder a los sitios de SharePoint o al contenido de OneDrive. Consulte el [panel de estado del servicio](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para comprobar si la organización está afectada.

- Los administradores de SharePoint y globales deben tener asignada una licencia de SharePoint. Es posible que las cuentas recién creadas con una licencia o rol de administrador de SharePoint tengan problemas al acceder a SharePoint, como "acceso denegado" o "no se encuentra el usuario". Espere al menos 24 horas para que la sincronización se complete en los sistemas. Sabemos que 24 horas puede parecer mucho tiempo. En muchos casos, ya estamos trabajando en una solución.

- Es posible que los usuarios de Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) reciban la denegación de acceso si el intervalo de tiempo de acceso permitido es muy pequeño, consulte [Acceso denegado a cuentas PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).