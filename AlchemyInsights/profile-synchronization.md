---
title: Sincronización de perfiles
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801786"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="e42a3-102">¿Cuándo se sincronizan mis cambios de perfil con la aplicación de Perfil de usuario de SharePoint?</span><span class="sxs-lookup"><span data-stu-id="e42a3-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="e42a3-103">SharePoint Online usa el trabajo del temporizador de importación de Active Directory (AD Import) para importar usuarios y grupos en la aplicación de Perfil de usuario.</span><span class="sxs-lookup"><span data-stu-id="e42a3-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="e42a3-104">La importación de AD sincroniza los cambios del almacén de directorio de SharePoint Online con la aplicación de Perfil de usuario.</span><span class="sxs-lookup"><span data-stu-id="e42a3-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="e42a3-105">Estos cambios se procesan por lotes.</span><span class="sxs-lookup"><span data-stu-id="e42a3-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="e42a3-106">El trabajo del temporizador se ejecuta hasta que se sincronicen los cambios.</span><span class="sxs-lookup"><span data-stu-id="e42a3-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="e42a3-107">El tiempo que tarda en ejecutarse el trabajo depende del número de cambios que se van a procesar.</span><span class="sxs-lookup"><span data-stu-id="e42a3-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="e42a3-108">Un gran número de cambios lleva más tiempo.</span><span class="sxs-lookup"><span data-stu-id="e42a3-108">A large number of changes takes longer.</span></span> <span data-ttu-id="e42a3-109">El contrato de nivel de servicio (SLA) indica que un cambio en un usuario en el directorio de SharePoint Online se reflejará en la aplicación de Perfil de usuario en 24 horas.</span><span class="sxs-lookup"><span data-stu-id="e42a3-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="e42a3-110">Más información sobre la sincronización de perfiles de usuario en SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e42a3-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

