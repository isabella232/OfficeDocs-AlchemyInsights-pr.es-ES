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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923148"
---
# <a name="rbac-rules"></a>Reglas RBAC

Si obtiene el error de permiso: 

- El cliente con identificador de objeto no tiene autorización para realizar acciones en el ámbito **(código: AuthorizationFailed):** cuando intente crear un recurso, compruebe que ha iniciado sesión actualmente con un usuario al que se le asigna un rol que tiene permiso de escritura para el recurso en el ámbito seleccionado. Por ejemplo, para administrar máquinas virtuales en un grupo de recursos, debe tener el rol Colaborador de máquina [virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) en el grupo de recursos (o ámbito primario). Para obtener una lista de los permisos para cada rol integrado, vea [Roles integrados para recursos de Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- No tiene permiso para crear una solicitud de soporte **técnico:** cuando intente crear o actualizar un vale de soporte técnico, compruebe que ha iniciado sesión actualmente con un usuario al que se le asigna un rol que tiene el permiso Microsoft.Support/supportTickets/write, como [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- No se pueden crear más asignaciones de roles **(código: RoleAssignmentLimitExceeded):** cuando intente asignar un rol, intente reducir el número de asignaciones de roles asignando roles a grupos en su lugar. Azure admite hasta **2000** asignaciones de roles por suscripción.

Para obtener más información sobre los roles RBAC de Azure, vea [Roles rbac de Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
