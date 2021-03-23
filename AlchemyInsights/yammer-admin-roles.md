---
title: Acerca de los administradores de Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995293"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="b10de-102">Acerca de los administradores de Yammer</span><span class="sxs-lookup"><span data-stu-id="b10de-102">About Yammer admins</span></span>

<span data-ttu-id="b10de-103">**Administradores de red**</span><span class="sxs-lookup"><span data-stu-id="b10de-103">**Network admins**</span></span>

<span data-ttu-id="b10de-104">Los administradores globales se promueven automáticamente al rol De administrador verificado en una red de Yammer.</span><span class="sxs-lookup"><span data-stu-id="b10de-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="b10de-105">En los siguientes casos, es posible que esta promoción no se produzca correctamente:</span><span class="sxs-lookup"><span data-stu-id="b10de-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="b10de-106">Existen varias redes de Yammer y el administrador ha iniciado sesión en la incorrecta.</span><span class="sxs-lookup"><span data-stu-id="b10de-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="b10de-107">[La consolidación](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) de red es necesaria para llegar a una red de Yammer.</span><span class="sxs-lookup"><span data-stu-id="b10de-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="b10de-108">Se está utilizando Pim de Azure.</span><span class="sxs-lookup"><span data-stu-id="b10de-108">Azure PIM is being used.</span></span> <span data-ttu-id="b10de-109">Es posible que el usuario no sea promovido a administrador global lo suficiente como para que se produzca la promoción.</span><span class="sxs-lookup"><span data-stu-id="b10de-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="b10de-110">Una actualización futura de Yammer puede resolver este problema, pero lo mejor es promover manualmente a los usuarios al administrador global.</span><span class="sxs-lookup"><span data-stu-id="b10de-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="b10de-111">Existe un problema de sincronización con la red de Yammer.</span><span class="sxs-lookup"><span data-stu-id="b10de-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="b10de-112">En este caso, se requiere una solicitud de soporte técnico para una investigación posterior.</span><span class="sxs-lookup"><span data-stu-id="b10de-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="b10de-113">Para obtener más información acerca de los roles de administrador de Yammer, vea [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="b10de-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="b10de-114">**Administradores de grupo**</span><span class="sxs-lookup"><span data-stu-id="b10de-114">**Group admins**</span></span>

<span data-ttu-id="b10de-115">Los administradores de grupos para grupos conectados de Microsoft 365 se sincronizan con la pertenencia a grupos de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b10de-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="b10de-116">Para grupos grandes, esta sincronización puede tardar un período prolongado.</span><span class="sxs-lookup"><span data-stu-id="b10de-116">For large groups, this sync can take an extended period.</span></span>
