---
title: Acerca de la identidad en Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146806"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="476f3-102">Acerca de la identidad en Yammer</span><span class="sxs-lookup"><span data-stu-id="476f3-102">About identity in Yammer</span></span>

<span data-ttu-id="476f3-103">Se recomienda que todas las redes realicen los siguientes pasos para evitar problemas relacionados con la identidad:</span><span class="sxs-lookup"><span data-stu-id="476f3-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="476f3-104">Exigir la identidad de Office 365 después de aprovisionar cuentas de Microsoft 365 para los usuarios en Azure AD con objeto de garantizar que todos los usuarios inicien sesión con su cuenta de Microsoft 365 principal.</span><span class="sxs-lookup"><span data-stu-id="476f3-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="476f3-105">Para obtener más información, vea [Exigir la identidad de Office 365 para usuarios de Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="476f3-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="476f3-106">Consolidar varias redes de Yammer.</span><span class="sxs-lookup"><span data-stu-id="476f3-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="476f3-107">Las configuraciones heredadas de Yammer permite conectar varias redes de Yammer a un espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="476f3-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="476f3-108">Para obtener más información, vea [Migración de red: consolidar varias redes de Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="476f3-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="476f3-109">Si lo desea, puede exigir licencias de Yammer para bloquear a los usuarios de Yammer en caso de que no tengan una licencia.</span><span class="sxs-lookup"><span data-stu-id="476f3-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="476f3-110">Para obtener más información, vea [Administrar licencias de usuario de Yammer en Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="476f3-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="476f3-111">Por último, auditar la lista de usuarios de las redes antiguas de Yammer y suspender a los usuarios antiguos.</span><span class="sxs-lookup"><span data-stu-id="476f3-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="476f3-112">Se recomienda que suspenda (desactive) a los usuarios en lugar de eliminarlos, ya que la eliminación es irreversible.</span><span class="sxs-lookup"><span data-stu-id="476f3-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="476f3-113">Para obtener más información, vea [Auditar usuarios de Yammer en redes conectadas a Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) y [Eliminar usuarios](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="476f3-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="476f3-114">Si configura Yammer siguiendo estos pasos, también estará listo para configurar la red de Yammer para el modo nativo de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="476f3-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="476f3-115">Para obtener más información, vea [Configurar su red de Yammer para el Modo nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="476f3-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>