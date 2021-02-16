---
title: Directiva de grupo
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
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243921"
---
# <a name="group-policy"></a><span data-ttu-id="6ac06-102">Directiva de grupo</span><span class="sxs-lookup"><span data-stu-id="6ac06-102">Group policy</span></span>

<span data-ttu-id="6ac06-103">La configuración de los objetos de usuario y equipo en Azure Active Directory Domain Services (Azure AD DS) suele administrarse con objetos de directiva de grupo (GPO).</span><span class="sxs-lookup"><span data-stu-id="6ac06-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="6ac06-104">Azure AD DS incluye GPO integrados para los usuarios de AADDC y los contenedores de equipos AADDC.</span><span class="sxs-lookup"><span data-stu-id="6ac06-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="6ac06-105">Puede personalizar estos GPO integrados para configurar las directivas de grupo según sea necesario para su entorno.</span><span class="sxs-lookup"><span data-stu-id="6ac06-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="6ac06-106">Los miembros del grupo de administradores de Azure AD DC tienen privilegios de administración de directivas de grupo en el dominio de Azure AD DS y también pueden crear GPO personalizados y unidades organizativas (OU).</span><span class="sxs-lookup"><span data-stu-id="6ac06-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="6ac06-107">Para obtener más información sobre qué es una directiva de grupo y cómo funciona, consulte la [Información general de la directiva de grupo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="6ac06-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="6ac06-108">En un entorno híbrido, las directivas de grupo configuradas en un entorno local de AD DS no se sincronizan con Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="6ac06-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="6ac06-109">Para definir opciones de configuración para usuarios o equipos en Azure AD DS, edite uno de los GPO predeterminados o cree uno personalizado.</span><span class="sxs-lookup"><span data-stu-id="6ac06-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="6ac06-110">El artículo [Administrar directiva de grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) le muestra cómo instalar las Herramientas de administración de directivas de grupo, editar los GPO integrados y crear GPO personalizados.</span><span class="sxs-lookup"><span data-stu-id="6ac06-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



