---
title: Varios usuarios obtienen un error de acceso denegado al agregar complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724380"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Varios usuarios obtienen un error de acceso denegado al agregar complementos en Outlook

Puede especificar qué administradores de su organización tienen permisos para instalar y administrar complementos para Outlook. También puede especificar qué usuarios de la organización tienen permiso para instalar y administrar los complementos para su propio uso.

Para más información, consulte [Especificar los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Para comprobar que ha asignado permisos para un usuario correctamente, reemplace <Role Name> por el nombre del rol para comprobar y ejecute el siguiente comando en Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

En este ejemplo se muestra cómo verificar a quién ha asignado permisos para instalar complementos de la Tienda Office para la organización.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

En los resultados, Get-ManagementRoleAssignment, revise las entradas de la columna Effective Users.

Para obtener información detallada acerca de la sintaxis y los parámetros, consulte [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 