---
title: Crear un grupo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816389"
---
# <a name="create-a-group"></a><span data-ttu-id="fbdac-102">Crear un grupo</span><span class="sxs-lookup"><span data-stu-id="fbdac-102">Create a group</span></span>

<span data-ttu-id="fbdac-103">En este tema se describe la creación de grupos.</span><span class="sxs-lookup"><span data-stu-id="fbdac-103">This topic describes group creation.</span></span>

<span data-ttu-id="fbdac-104">**Permiso para crear un grupo**</span><span class="sxs-lookup"><span data-stu-id="fbdac-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="fbdac-105">Asegúrese de que está autorizado a crear un nuevo grupo.</span><span class="sxs-lookup"><span data-stu-id="fbdac-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="fbdac-106">Los administradores globales pueden deshabilitar la creación de grupos en Azure Portal o el Panel de acceso.</span><span class="sxs-lookup"><span data-stu-id="fbdac-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="fbdac-107">Puede que necesite que un administrador cree el nuevo grupo o que le conceda los permisos adecuados.</span><span class="sxs-lookup"><span data-stu-id="fbdac-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="fbdac-108">**Administrar los permisos de creación de grupos**</span><span class="sxs-lookup"><span data-stu-id="fbdac-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="fbdac-109">Los administradores globales pueden administrar permisos de creación de grupos (por motivos relacionados con la seguridad) u grupos de Office 365 creados en Azure Portal o el Panel de acceso, seleccionando "Los usuarios pueden crear grupos de seguridad en Azure Portals" o "Los usuarios pueden crear grupos de Office 365 en Azure Portals" en Todos los grupos  >  **Generales (Configuración).**</span><span class="sxs-lookup"><span data-stu-id="fbdac-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="fbdac-110">También puede restringir la creación de grupos para seleccionar un grupo de usuarios si tiene una licencia de Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="fbdac-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="fbdac-111">**Deshabilitar la notificación de bienvenida para los nuevos miembros del grupo de Office 365**</span><span class="sxs-lookup"><span data-stu-id="fbdac-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="fbdac-112">La notificación de bienvenida enviada a los usuarios que se agregan a grupos de Office 365 se puede deshabilitar estableciendo **UnifiedGroupWelcomeMessageEnabled** en False en Powershell.</span><span class="sxs-lookup"><span data-stu-id="fbdac-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="fbdac-113">Obtenga información sobre esta configuración [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="fbdac-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

