---
title: Crear un grupo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086394"
---
# <a name="create-a-group"></a><span data-ttu-id="249e6-102">Crear un grupo</span><span class="sxs-lookup"><span data-stu-id="249e6-102">Create a group</span></span>

<span data-ttu-id="249e6-103">En este tema se describe la creación de grupos.</span><span class="sxs-lookup"><span data-stu-id="249e6-103">This topic describes group creation.</span></span>

<span data-ttu-id="249e6-104">**Permiso para crear un grupo**</span><span class="sxs-lookup"><span data-stu-id="249e6-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="249e6-105">Asegúrese de que tiene autorización para crear un nuevo grupo.</span><span class="sxs-lookup"><span data-stu-id="249e6-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="249e6-106">Los administradores globales pueden deshabilitar la creación de grupos en el panel de acceso o el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="249e6-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="249e6-107">Es posible que necesite un administrador para crear el nuevo grupo o para concederle los permisos adecuados.</span><span class="sxs-lookup"><span data-stu-id="249e6-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="249e6-108">**Administrar permisos de creación de grupos**</span><span class="sxs-lookup"><span data-stu-id="249e6-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="249e6-109">Los administradores globales pueden administrar los permisos de creación de grupos (por motivos relacionados con la seguridad) o los grupos de Office 365 creados en el portal de Azure o en el panel de acceso, seleccionando "los usuarios pueden crear grupos de seguridad en los portales de Azure" o "los usuarios pueden crear grupos de Office 365 en Azure portales" en **todos los grupos**  >  **General (configuración)**.</span><span class="sxs-lookup"><span data-stu-id="249e6-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="249e6-110">También puede restringir la creación de grupos para seleccionar un grupo de usuarios si tiene una licencia de Azure Premium de Active Directory P1.</span><span class="sxs-lookup"><span data-stu-id="249e6-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="249e6-111">**Deshabilitar la notificación de bienvenida para nuevos miembros del grupo de Office 365**</span><span class="sxs-lookup"><span data-stu-id="249e6-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="249e6-112">La notificación de bienvenida que se envía a los usuarios que se agregan a los grupos de Office 365 se puede deshabilitar si se establece **UnifiedGroupWelcomeMessageEnabled** en false en PowerShell.</span><span class="sxs-lookup"><span data-stu-id="249e6-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="249e6-113">Obtenga información [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)sobre esta configuración.</span><span class="sxs-lookup"><span data-stu-id="249e6-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

