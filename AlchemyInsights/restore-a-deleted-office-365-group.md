---
title: Restaurar un grupo de Microsoft 365 eliminado
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597460"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="09024-102">Restaurar un grupo de Microsoft 365 eliminado</span><span class="sxs-lookup"><span data-stu-id="09024-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="09024-103">Puede restaurar un grupo eliminado de Microsoft 365 o Microsoft Teams en un plazo de 30 días desde la eliminación.</span><span class="sxs-lookup"><span data-stu-id="09024-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="09024-104">Vaya al Centro [de administración de Microsoft 365](https://aka.ms/RestoreDeletedGroup) para iniciar sesión y enumerar los grupos y equipos eliminados.</span><span class="sxs-lookup"><span data-stu-id="09024-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="09024-105">**Nota:** Inicie sesión con la cuenta asignada al administrador de inquilinos o al rol de administrador de grupos.</span><span class="sxs-lookup"><span data-stu-id="09024-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="09024-106">Seleccione el grupo de Microsoft 365 eliminado/Teams que desea restaurar y haga clic en **Restaurar grupo**.</span><span class="sxs-lookup"><span data-stu-id="09024-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="09024-107">Si el grupo no se puede restaurar debido a una dirección SMTP en conflicto, use el siguiente comando para buscar el objeto que está provocando conflictos y quitar la dirección SMTP:</span><span class="sxs-lookup"><span data-stu-id="09024-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="09024-108">**Nota:** En algunos casos, el grupo y todos sus datos pueden tardar hasta 24 horas en restaurarse.</span><span class="sxs-lookup"><span data-stu-id="09024-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="09024-109">Para obtener más información o aprender a restaurar grupos con PowerShell, vea [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="09024-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>