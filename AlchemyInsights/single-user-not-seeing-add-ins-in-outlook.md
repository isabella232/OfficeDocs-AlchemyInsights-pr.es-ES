---
title: Un solo usuario no ve complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154604"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="a81c8-102">Un solo usuario no ve complementos en Outlook</span><span class="sxs-lookup"><span data-stu-id="a81c8-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="a81c8-103">El usuario puede ser parte de un rol que no tenga el parámetro AppsForOfficeEnabled correcto.</span><span class="sxs-lookup"><span data-stu-id="a81c8-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="a81c8-104">Ejecute este cmdlet para averiguar si el rol correcto está asociado al usuario:</span><span class="sxs-lookup"><span data-stu-id="a81c8-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="a81c8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="a81c8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="a81c8-106">Para más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="a81c8-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
