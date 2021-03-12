---
title: Solucionar problemas de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704911"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="23d4e-102">Solucionar problemas de acceso denegado</span><span class="sxs-lookup"><span data-stu-id="23d4e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="23d4e-103">Si alguien recibió un mensaje "Acceso denegado" a una carpeta compartida en SharePoint, es posible que el administrador de la colección de sitios haya habilitado "Modo de bloqueo de permisos de usuario de acceso limitado".</span><span class="sxs-lookup"><span data-stu-id="23d4e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="23d4e-104">Para desactivar esto:</span><span class="sxs-lookup"><span data-stu-id="23d4e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="23d4e-105">Vaya al sitio, haga clic en el icono Configuración y, a continuación, haga clic en **Configuración del sitio**.</span><span class="sxs-lookup"><span data-stu-id="23d4e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="23d4e-106">En **Administración de la colección de sitios**, haga clic en **Características de la colección de sitios**.</span><span class="sxs-lookup"><span data-stu-id="23d4e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="23d4e-107">Junto al modo de bloqueo de permisos de usuario de acceso **limitado,** haga clic **en Desactivar**.</span><span class="sxs-lookup"><span data-stu-id="23d4e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="23d4e-108">También se puede producir un mensaje de acceso denegado para carpetas compartidas si el sitio es un sitio de publicación.</span><span class="sxs-lookup"><span data-stu-id="23d4e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="23d4e-109">Para obtener información, consulta [Acceso denegado al acceder a una carpeta compartida.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="23d4e-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="23d4e-110">Si alguien recibió un mensaje de "Acceso denegado" al intentar ver solicitudes de acceso, el usuario debe agregarse como administrador de la colección de sitios o como miembro del grupo Propietarios del sitio.</span><span class="sxs-lookup"><span data-stu-id="23d4e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="23d4e-111">Para obtener más información, [consulta Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="23d4e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="23d4e-112">Si un usuario recibió un mensaje de "Acceso denegado" después de que se quitara de Active Directory localmente y, a continuación, se agregara de nuevo, vea [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="23d4e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

