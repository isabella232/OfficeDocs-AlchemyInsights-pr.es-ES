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
# <a name="rbac-rules"></a><span data-ttu-id="fab5c-102">Reglas de RBAC</span><span class="sxs-lookup"><span data-stu-id="fab5c-102">RBAC rules</span></span>

<span data-ttu-id="fab5c-103">Si recibe el error de permiso:</span><span class="sxs-lookup"><span data-stu-id="fab5c-103">If you get the permission error:</span></span> 

- <span data-ttu-id="fab5c-104">**El cliente con el identificador de objeto no tiene autorización para realizar acciones sobre el ámbito (código: AuthorizationFailed)**: cuando intenta crear un recurso, compruebe que actualmente ha iniciado sesión con un usuario que tiene asignado un rol que tiene permiso de escritura en el recurso en el ámbito seleccionado.</span><span class="sxs-lookup"><span data-stu-id="fab5c-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="fab5c-105">Por ejemplo, para administrar máquinas virtuales en un grupo de recursos, debe tener el rol de [colaborador de máquina virtual](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) en el grupo de recursos (o ámbito primario).</span><span class="sxs-lookup"><span data-stu-id="fab5c-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="fab5c-106">Para obtener una lista de los permisos de cada rol integrado, vea [roles integrados para recursos de Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fab5c-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="fab5c-107">**No tiene permiso para crear una solicitud de soporte técnico**: cuando intenta crear o actualizar un vale de soporte técnico, compruebe que actualmente ha iniciado sesión con un usuario que tiene asignado un rol con el permiso Microsoft. support/supportTickets/Write, como [support request Contribution](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="fab5c-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="fab5c-108">**No se pueden crear más asignaciones de funciones (código: RoleAssignmentLimitExceeded)**: cuando intenta asignar una función, intente reducir el número de asignaciones de funciones mediante la asignación de funciones a grupos en su lugar.</span><span class="sxs-lookup"><span data-stu-id="fab5c-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="fab5c-109">Azure admite hasta **2000** asignaciones de roles por suscripción.</span><span class="sxs-lookup"><span data-stu-id="fab5c-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="fab5c-110">Para obtener más información sobre los roles RBAC de Azure, consulte [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fab5c-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
