---
title: 'Roles RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576624"
---
# <a name="rbac-rules"></a>Reglas de RBAC

Si recibe el error de permiso: 

- **El cliente con el identificador de objeto no tiene autorización para realizar acciones sobre el ámbito (código: AuthorizationFailed)**: cuando intenta crear un recurso, compruebe que actualmente ha iniciado sesión con un usuario que tiene asignado un rol que tiene permiso de escritura en el recurso en el ámbito seleccionado. Por ejemplo, para administrar máquinas virtuales en un grupo de recursos, debe tener el rol de [colaborador de máquina virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) en el grupo de recursos (o ámbito primario). Para obtener una lista de los permisos de cada rol integrado, vea [roles integrados para recursos de Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **No tiene permiso para crear una solicitud de soporte técnico**: cuando intenta crear o actualizar un vale de soporte técnico, compruebe que actualmente ha iniciado sesión con un usuario que tiene asignado un rol con el permiso Microsoft. support/supportTickets/Write, como [support request Contribution](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **No se pueden crear más asignaciones de funciones (código: RoleAssignmentLimitExceeded)**: cuando intenta asignar una función, intente reducir el número de asignaciones de funciones mediante la asignación de funciones a grupos en su lugar. Azure admite hasta **2000** asignaciones de roles por suscripción.

Para obtener más información sobre los roles RBAC de Azure, consulte [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
