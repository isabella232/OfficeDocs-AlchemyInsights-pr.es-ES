---
title: Sincronización de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243922"
---
# <a name="group-sync"></a><span data-ttu-id="6f8a0-102">Sincronización de grupo</span><span class="sxs-lookup"><span data-stu-id="6f8a0-102">Group sync</span></span>

<span data-ttu-id="6f8a0-103">En este artículo se proporcionan instrucciones sobre la sincronización de grupos.</span><span class="sxs-lookup"><span data-stu-id="6f8a0-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="6f8a0-104">Si un administrador global o un propietario del grupo no puede modificar las propiedades del grupo, agregar miembros o asignar propietarios en Azure Portal, asegúrese de que el origen de la autoridad del grupo es Azure Active Directory (Azure AD) para que el administrador global o el propietario del grupo modifique el grupo.</span><span class="sxs-lookup"><span data-stu-id="6f8a0-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="6f8a0-105">Antes de intentar eliminar un grupo sincronizado en Azure AD, asegúrese de haber [eliminado todas las licencias asignadas](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) para evitar errores.</span><span class="sxs-lookup"><span data-stu-id="6f8a0-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="6f8a0-106">Para información sobre cómo sincronizar usuarios, grupos y contactos, vea [Sincronización de Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts) y siga las indicaciones de [Sincronizar un grupo local con Azure mediante Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) para sincronizar grupos locales con AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6f8a0-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="6f8a0-107">Siga la guía [Solución de problemas durante la sincronización](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) para solucionar problemas comunes durante la sincronización.</span><span class="sxs-lookup"><span data-stu-id="6f8a0-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

