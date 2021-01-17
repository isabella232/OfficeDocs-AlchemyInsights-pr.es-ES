---
title: Asignar grupos a un rol de Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875456"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="99206-102">Asignar grupos a un rol de Azure AD</span><span class="sxs-lookup"><span data-stu-id="99206-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="99206-103">Para asignar un grupo de Azure AD con origen de autoridad en Azure AD a un rol de Azure AD, siga los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="99206-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="99206-104">Crear grupo - Para crear un grupo nuevo:</span><span class="sxs-lookup"><span data-stu-id="99206-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="99206-105">a.</span><span class="sxs-lookup"><span data-stu-id="99206-105">a.</span></span> <span data-ttu-id="99206-106">Inicie sesión en el Centro de administración de Azure AD con los permisos de **rol de administración con privilegios** o de **administrador global**.</span><span class="sxs-lookup"><span data-stu-id="99206-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="99206-107">b.</span><span class="sxs-lookup"><span data-stu-id="99206-107">b.</span></span> <span data-ttu-id="99206-108">Seleccione **Azure Active Directory > Grupos > Todos los grupos > Nuevo grupo**.</span><span class="sxs-lookup"><span data-stu-id="99206-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="99206-109">c.</span><span class="sxs-lookup"><span data-stu-id="99206-109">c.</span></span> <span data-ttu-id="99206-110">Cree el grupo.</span><span class="sxs-lookup"><span data-stu-id="99206-110">Create the group.</span></span>

2. <span data-ttu-id="99206-111">Puede asignar el rol al grupo durante la creación del grupo o después de crearlo.</span><span class="sxs-lookup"><span data-stu-id="99206-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="99206-112">a.</span><span class="sxs-lookup"><span data-stu-id="99206-112">a.</span></span> <span data-ttu-id="99206-113">Para asignar un rol al grupo en el momento de crearlo, cambie el botón de alternancia a **Los roles de Azure AD se pueden asignar al grupo** y cree el grupo.</span><span class="sxs-lookup"><span data-stu-id="99206-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="99206-114">b.</span><span class="sxs-lookup"><span data-stu-id="99206-114">b.</span></span> <span data-ttu-id="99206-115">Para asignar un rol al grupo después de creado, vaya a la pestaña **Roles asignados** del grupo recién creado y asigne el rol al grupo.</span><span class="sxs-lookup"><span data-stu-id="99206-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="99206-116">**Administrar la suscripción a un grupo asignado al rol de Azure AD**</span><span class="sxs-lookup"><span data-stu-id="99206-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="99206-117">Para evitar la elevación de privilegios, de forma predeterminada, solo los administradores de roles con privilegios y los administradores globales pueden modificar la pertenencia a un grupo que esté asignado a un rol.</span><span class="sxs-lookup"><span data-stu-id="99206-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="99206-118">En cambio, puede asignar un propietario a este grupo y delegar esta tarea.</span><span class="sxs-lookup"><span data-stu-id="99206-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="99206-119">Para obtener más información sobre cómo asignar grupos en la nube a roles de Azure AD, vea [Asignar roles de AD a grupos en la nube](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="99206-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="99206-120">Para obtener más información sobre cómo solucionar problemas de roles asignados a grupos en la nube, vea [Solución de problemas de roles asignados a grupos en la nube](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="99206-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





