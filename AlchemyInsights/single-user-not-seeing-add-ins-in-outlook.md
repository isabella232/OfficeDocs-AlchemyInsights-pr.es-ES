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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Un solo usuario no ve complementos en Outlook

El usuario puede ser parte de un rol que no tenga el parámetro AppsForOfficeEnabled correcto. Ejecute este cmdlet para averiguar si el rol correcto está asociado al usuario:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Para más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
