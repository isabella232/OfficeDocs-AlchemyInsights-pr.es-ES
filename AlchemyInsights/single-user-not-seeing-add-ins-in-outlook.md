---
title: Un solo usuario no ve complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050675"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Un solo usuario no ve complementos en Outlook

El usuario puede ser parte de un rol que no tenga el parámetro AppsForOfficeEnabled correcto. Ejecute este cmdlet para averiguar si el rol correcto está asociado al usuario:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Para más información, consulte [Especifique los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
