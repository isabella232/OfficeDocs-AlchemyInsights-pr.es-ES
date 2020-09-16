---
title: OneDrive para la empresa web OneDrive redirige a Delve
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776397"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="5beb9-102">Se redirige a Delve después de hacer clic en OneDrive</span><span class="sxs-lookup"><span data-stu-id="5beb9-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="5beb9-103">Consulte nuestra guía detallada de [solución de problemas](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="5beb9-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="5beb9-104">Para resolver este problema, el administrador debe conceder a los usuarios el derecho a crear su sitio de mis sitios.</span><span class="sxs-lookup"><span data-stu-id="5beb9-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="5beb9-105">Esto se debe a que la página de OneDrive para la empresa se crea en mis sitios.</span><span class="sxs-lookup"><span data-stu-id="5beb9-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="5beb9-106">Para conceder este derecho, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="5beb9-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="5beb9-107">En el centro de administración de SharePoint, haga clic en **perfiles de usuario**.</span><span class="sxs-lookup"><span data-stu-id="5beb9-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="5beb9-108">En la sección **personas** , haga clic en **administrar permisos de usuario**.</span><span class="sxs-lookup"><span data-stu-id="5beb9-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="5beb9-109">Agregar usuarios que requieren permisos para crear su sitio mis sitios.</span><span class="sxs-lookup"><span data-stu-id="5beb9-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="5beb9-110">De forma predeterminada, esta opción está establecida en **todos excepto los usuarios externos**.</span><span class="sxs-lookup"><span data-stu-id="5beb9-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="5beb9-111">Una vez que haya agregado el usuario, los usuarios o el grupo, asegúrese de que se haya seleccionado el usuario, los usuarios o el grupo agregado, desplácese a la sección **permisos** y, a continuación, active la casilla junto a **crear sitio personal (necesario para el almacenamiento personal, el suministro de noticias y el contenido seguido)**.</span><span class="sxs-lookup"><span data-stu-id="5beb9-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="5beb9-112">Haga clic en **Aceptar**y, a continuación, haga que el usuario vaya a la página de OneDrive para crear el sitio.</span><span class="sxs-lookup"><span data-stu-id="5beb9-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
