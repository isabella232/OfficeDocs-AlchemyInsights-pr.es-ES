---
title: Problemas con el uso de la consola de administración de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728304"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="a32ff-102">Problemas con el uso de la consola de administración de Intune</span><span class="sxs-lookup"><span data-stu-id="a32ff-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="a32ff-103">**"Acceso denegado" al navegar por el portal de administración de Intune.**</span><span class="sxs-lookup"><span data-stu-id="a32ff-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="a32ff-104">Si es miembro de un rol personalizado de Intune, asegúrese de que se ha asignado una licencia de Intune o de Enterprise Mobility Suite (EMS) a su cuenta.</span><span class="sxs-lookup"><span data-stu-id="a32ff-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="a32ff-105">Si usa Configuration Manager para administrar dispositivos, compruebe que usted no forma parte del conjunto de usuarios de Intune para la MDM de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="a32ff-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="a32ff-106">Compruebe que se le han asignado los permisos adecuados de control de administración basado en roles (RBAC) en la hoja de roles de Intune.</span><span class="sxs-lookup"><span data-stu-id="a32ff-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="a32ff-107">Compruebe que el grupo usado no es una lista de distribución.</span><span class="sxs-lookup"><span data-stu-id="a32ff-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="a32ff-108">Intune en el Microsoft Azure Portal solo admite cuentas de usuario que pertenecen a grupos de seguridad de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a32ff-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="a32ff-109">Revisar los grupos en el portal de Azure > **Intune** > **Grupos**, o en Microsoft Azure Portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="a32ff-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="a32ff-110">**El usuario tiene demasiados permisos para la función Intune asignada**</span><span class="sxs-lookup"><span data-stu-id="a32ff-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="a32ff-111">Aconseje al usuario que vaya a **Intune** > **Roles de Intune** > **Mis permisos** > **Exportar** para revisar los permisos concedidos.</span><span class="sxs-lookup"><span data-stu-id="a32ff-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="a32ff-112">**He agregado un grupo de ámbito a un rol, pero los usuarios de ese rol aún ven a otros usuarios o dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="a32ff-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="a32ff-113">Los grupos de ámbito no filtran usuarios o dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a32ff-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="a32ff-114">Grupos de ámbito:</span><span class="sxs-lookup"><span data-stu-id="a32ff-114">Scope groups:</span></span>

- <span data-ttu-id="a32ff-115">Limitar qué usuarios pueden asignar directivas o aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="a32ff-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="a32ff-116">Permitir que solo usuarios específicos ejecuten tareas remotas en dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a32ff-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="a32ff-117">Para obtener más información sobre los grupos de ámbito, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="a32ff-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="a32ff-118">**Agregué un usuario a un rol de Intune, pero aún tienen acceso total a la consola de administración de Intune.**</span><span class="sxs-lookup"><span data-stu-id="a32ff-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="a32ff-119">Desplácese hasta Intune > **Usuarios** en el Microsoft Azure Portal y compruebe que el usuario no tiene asignado ninguno de los siguientes roles en el portal de Azure:</span><span class="sxs-lookup"><span data-stu-id="a32ff-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="a32ff-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a32ff-120">Global administrator</span></span>
- <span data-ttu-id="a32ff-121">Administrador de servicios de Intune</span><span class="sxs-lookup"><span data-stu-id="a32ff-121">Intune service administrator</span></span>
- <span data-ttu-id="a32ff-122">Administrador de SharePoint</span><span class="sxs-lookup"><span data-stu-id="a32ff-122">SharePoint administrator</span></span>

<span data-ttu-id="a32ff-123">Para más información, consulte [Control de acceso basado en roles (RBAC) con Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="a32ff-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="a32ff-124">**Problemas de acceso**</span><span class="sxs-lookup"><span data-stu-id="a32ff-124">**Access Issues**</span></span>

<span data-ttu-id="a32ff-125">Para más información, consulte [No puedo iniciar sesión en Office 365, Azure o Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="a32ff-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>