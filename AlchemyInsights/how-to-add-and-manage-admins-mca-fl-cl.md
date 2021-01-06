---
title: Cómo agregar y administrar administradores
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755528"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="7604d-102">Cómo agregar y administrar administradores</span><span class="sxs-lookup"><span data-stu-id="7604d-102">How to add and manage admins</span></span>

<span data-ttu-id="7604d-103">En función de la descripción del problema, hemos encontrado una soluci? a para usted.</span><span class="sxs-lookup"><span data-stu-id="7604d-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="7604d-104">La mayoría de los clientes pudieron resolver su problema por su cuenta después de seguir la documentación.</span><span class="sxs-lookup"><span data-stu-id="7604d-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="7604d-105">Para administrar su cuenta de facturación para un acuerdo de cliente de Microsoft (MCA), puede usar diferentes roles con el nivel de acceso deseado.</span><span class="sxs-lookup"><span data-stu-id="7604d-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="7604d-106">Estos roles se agregan además de los roles de servicio de Azure integrados que le ayudarán a controlar los recursos.</span><span class="sxs-lookup"><span data-stu-id="7604d-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="7604d-107">**Para agregar roles de facturación en Azure Portal:**</span><span class="sxs-lookup"><span data-stu-id="7604d-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="7604d-108">Inicie sesión en el [portal de Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7604d-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7604d-109">Buscar la *Administración de costos + facturación*.</span><span class="sxs-lookup"><span data-stu-id="7604d-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="7604d-110">Seleccione control de acceso (IAM) en un ámbito como la cuenta de facturación, el perfil de facturación o la sección de facturas donde desea dar acceso.</span><span class="sxs-lookup"><span data-stu-id="7604d-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="7604d-111">La página control de acceso (IAM) enumera los usuarios y grupos que se asignan a cada rol para ese ámbito.</span><span class="sxs-lookup"><span data-stu-id="7604d-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="7604d-112">Para conceder acceso a un usuario, seleccione **Agregar** desde la parte superior de la página.</span><span class="sxs-lookup"><span data-stu-id="7604d-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="7604d-113">En la lista desplegable *rol* , seleccione un rol.</span><span class="sxs-lookup"><span data-stu-id="7604d-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="7604d-114">Escriba la dirección de correo electrónico del usuario al que desea conceder acceso.</span><span class="sxs-lookup"><span data-stu-id="7604d-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="7604d-115">Seleccione **Guardar** para asignar el rol.</span><span class="sxs-lookup"><span data-stu-id="7604d-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="7604d-116">Para quitar el acceso de un usuario, seleccione el usuario con la asignación de roles que desea quitar.</span><span class="sxs-lookup"><span data-stu-id="7604d-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="7604d-117">Seleccione **quitar**.</span><span class="sxs-lookup"><span data-stu-id="7604d-117">Select **Remove**.</span></span>

<span data-ttu-id="7604d-118">**Documentos recomendados**</span><span class="sxs-lookup"><span data-stu-id="7604d-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="7604d-119">Definiciones de roles de facturación</span><span class="sxs-lookup"><span data-stu-id="7604d-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="7604d-120">Roles y tareas de la cuenta de facturación</span><span class="sxs-lookup"><span data-stu-id="7604d-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="7604d-121">Introducción a su cuenta de facturación de MCA</span><span class="sxs-lookup"><span data-stu-id="7604d-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="7604d-122">Comprobar el acceso a un acuerdo de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="7604d-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
