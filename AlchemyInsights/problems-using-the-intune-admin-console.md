---
title: Problemas con el uso de la consola de administración de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "46523057"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="ffd5c-102">Problemas con el uso de la consola de administración de Intune</span><span class="sxs-lookup"><span data-stu-id="ffd5c-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="ffd5c-103">**"Acceso denegado" al navegar por el portal de administración de Intune.**</span><span class="sxs-lookup"><span data-stu-id="ffd5c-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="ffd5c-104">Si es miembro de un rol personalizado de Intune, asegúrese de que se ha asignado una licencia de Intune o de Enterprise Mobility Suite (EMS) a su cuenta.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="ffd5c-105">Si usa Configuration Manager para administrar dispositivos, compruebe que usted no forma parte del conjunto de usuarios de Intune para la MDM de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="ffd5c-106">Compruebe que se le han asignado los permisos adecuados de control de administración basado en roles (RBAC) en la hoja de roles de Intune.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="ffd5c-107">Compruebe que el grupo usado no es una lista de distribución.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="ffd5c-108">Intune en el Microsoft Azure Portal solo admite cuentas de usuario que pertenecen a grupos de seguridad de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="ffd5c-109">Revisar los grupos en el portal de Azure > **Intune** > **Grupos**, o en Microsoft Azure Portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="ffd5c-110">**El usuario tiene demasiados permisos para la función Intune asignada**</span><span class="sxs-lookup"><span data-stu-id="ffd5c-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="ffd5c-111">Aconseje al usuario que vaya a **Intune** > **Roles de Intune** > **Mis permisos** > **Exportar** para revisar los permisos concedidos.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="ffd5c-112">**He agregado un grupo de ámbito a un rol, pero los usuarios de ese rol aún ven a otros usuarios o dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="ffd5c-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="ffd5c-113">Los grupos de ámbito no filtran usuarios o dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="ffd5c-114">Grupos de ámbito:</span><span class="sxs-lookup"><span data-stu-id="ffd5c-114">Scope groups:</span></span>

- <span data-ttu-id="ffd5c-115">Limitar qué usuarios pueden asignar directivas o aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="ffd5c-116">Permitir que solo usuarios específicos ejecuten tareas remotas en dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ffd5c-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="ffd5c-117">Para obtener más información sobre los grupos de ámbito, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ffd5c-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ffd5c-118">**Agregué un usuario a un rol de Intune, pero aún tienen acceso total a la consola de administración de Intune.**</span><span class="sxs-lookup"><span data-stu-id="ffd5c-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="ffd5c-119">Desplácese hasta Intune > **Usuarios** en el Microsoft Azure Portal y compruebe que el usuario no tiene asignado ninguno de los siguientes roles en el portal de Azure:</span><span class="sxs-lookup"><span data-stu-id="ffd5c-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="ffd5c-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ffd5c-120">Global administrator</span></span>
- <span data-ttu-id="ffd5c-121">Administrador de servicios de Intune</span><span class="sxs-lookup"><span data-stu-id="ffd5c-121">Intune service administrator</span></span>
- <span data-ttu-id="ffd5c-122">Administrador de SharePoint</span><span class="sxs-lookup"><span data-stu-id="ffd5c-122">SharePoint administrator</span></span>

<span data-ttu-id="ffd5c-123">Para más información, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ffd5c-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ffd5c-124">**Problemas de acceso**</span><span class="sxs-lookup"><span data-stu-id="ffd5c-124">**Access Issues**</span></span>

<span data-ttu-id="ffd5c-125">Para más información, consulte [No puedo iniciar sesión en Office 365, Azure o Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="ffd5c-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>