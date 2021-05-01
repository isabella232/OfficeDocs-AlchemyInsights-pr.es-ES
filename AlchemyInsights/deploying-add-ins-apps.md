---
title: Implementación de complementos para Aplicaciones Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107555"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Implementación de complementos para Aplicaciones Microsoft 365

La implementación centralizada es la forma recomendada para implementar Office complementos para usuarios y grupos de la organización. Para implementar complementos, siga los pasos siguientes:

**Nota:** Para instalar complementos para Office como un usuario individual, vea [Ver,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)administrar e instalar complementos en Office programas . Además, asegúrate de que la adquisición individual de Office complementos de la Tienda está habilitada. 

1. Asegúrese de que el entorno cumple los requisitos para la implementación de complementos mediante la implementación centralizada. Para obtener más información, vea [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Ve a **Configuración** aplicaciones integradas Obtener aplicaciones en  >    >   el centro Microsoft 365 administración para implementar complementos. 

Notas: 

- Las aplicaciones integradas requieren que el administrador tenga permisos de administrador global Exchange administrador.

- Al implementar complementos para varios usuarios, se recomienda realizar asignaciones mediante grupos en lugar de usuarios individuales. Para obtener más información, vea [Consideraciones al asignar un complemento a usuarios y grupos](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- La implementación centralizada no admite usuarios de grupos anidados o grupos que tienen grupos primarios. Para obtener más información, vea [Asignaciones de usuarios y grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Asegúrese de que Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') esté habilitado para que los usuarios inicien sesión. Para obtener más información, consulta [Configurar las propiedades de la aplicación.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Si tiene problemas para implementar complementos mediante aplicaciones integradas, intente implementar mediante [complementos](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Para más información, vea:

[Implementar complementos en el Centro de administración](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrar complementos en el Centro de administración](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Usar los cmdlets de PowerShell de implementación centralizada para administrar complementos](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office complementos mediante](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) la implementación centralizada a través del Centro Microsoft 365 administración 
 [Solución de problemas: el usuario no ve complementos](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Solucionar errores de usuario con Office complementos](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)