---
title: Administrar grupos de aplicaciones con Azure portal para escritorio virtual de Windows
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
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715720"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="c59e8-102">Administrar grupos de aplicaciones con Azure portal para escritorio virtual de Windows</span><span class="sxs-lookup"><span data-stu-id="c59e8-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="c59e8-103">El grupo de aplicaciones predeterminado creado para un nuevo grupo host de escritorio virtual de Windows también publica el escritorio completo.</span><span class="sxs-lookup"><span data-stu-id="c59e8-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="c59e8-104">Además, el uso del portal de Azure le permite crear uno o más grupos de aplicaciones de RemoteApp para el grupo de hosts.</span><span class="sxs-lookup"><span data-stu-id="c59e8-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="c59e8-105">El proceso de implementación hará lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="c59e8-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="c59e8-106">Cree el grupo de aplicaciones RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="c59e8-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="c59e8-107">Agregue las aplicaciones seleccionadas al grupo de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="c59e8-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="c59e8-108">Publique usuarios individuales o grupos de usuarios en el grupo de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="c59e8-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="c59e8-109">Registre el grupo de aplicaciones, si decide hacerlo.</span><span class="sxs-lookup"><span data-stu-id="c59e8-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="c59e8-110">Cree un vínculo a una plantilla de Azure Resource Manager de acuerdo con la configuración, que puede descargar y guardar.</span><span class="sxs-lookup"><span data-stu-id="c59e8-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="c59e8-111">Para crear un grupo de RemoteApp para el escritorio virtual de Windows, siga las instrucciones que se indican en [Manage App Groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span><span class="sxs-lookup"><span data-stu-id="c59e8-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
