---
title: Varios usuarios obtienen un error de acceso denegado al agregar complementos en Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397750"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="51a13-102">Varios usuarios obtienen un error de acceso denegado al agregar complementos en Outlook</span><span class="sxs-lookup"><span data-stu-id="51a13-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="51a13-103">Puede especificar qué administradores de su organización tienen permisos para instalar y administrar complementos para Outlook.</span><span class="sxs-lookup"><span data-stu-id="51a13-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="51a13-104">También puede especificar qué usuarios de la organización tienen permiso para instalar y administrar los complementos para su propio uso.</span><span class="sxs-lookup"><span data-stu-id="51a13-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="51a13-105">Para más información, consulte [Especificar los administradores y los usuarios que pueden instalar y administrar complementos para Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="51a13-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="51a13-106">Para comprobar que ha asignado permisos para un usuario correctamente, reemplace <Role Name> por el nombre del rol para comprobar y ejecute el siguiente comando en Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="51a13-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="51a13-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="51a13-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="51a13-108">En este ejemplo se muestra cómo verificar a quién ha asignado permisos para instalar complementos de la Tienda Office para la organización.</span><span class="sxs-lookup"><span data-stu-id="51a13-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="51a13-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="51a13-109">PowerShell</span></span>

<span data-ttu-id="51a13-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="51a13-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="51a13-111">En los resultados, Get-ManagementRoleAssignment, revise las entradas de la columna Effective Users.</span><span class="sxs-lookup"><span data-stu-id="51a13-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="51a13-112">Para obtener información detallada acerca de la sintaxis y los parámetros, consulte [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="51a13-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 