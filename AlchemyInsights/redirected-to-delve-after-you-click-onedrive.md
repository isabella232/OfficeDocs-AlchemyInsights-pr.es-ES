---
title: OneDrive para la Empresa Web OneDrive redirige a Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800006"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="28d77-102">Redirigido a Delve después de hacer clic en OneDrive</span><span class="sxs-lookup"><span data-stu-id="28d77-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="28d77-103">Consulte nuestra guía de [solución de problemas detallada.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="28d77-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="28d77-104">Para resolver este problema, el administrador debe conceder a los usuarios el derecho de crear su sitio de Mis sitios.</span><span class="sxs-lookup"><span data-stu-id="28d77-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="28d77-105">Esto se debe a que la página de OneDrive para la Empresa se crea en Mis sitios.</span><span class="sxs-lookup"><span data-stu-id="28d77-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="28d77-106">Para conceder este derecho, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="28d77-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="28d77-107">En el Centro de administración de SharePoint, haga clic **en Perfiles de usuario**.</span><span class="sxs-lookup"><span data-stu-id="28d77-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="28d77-108">En la **sección Personas,** haga clic **en Administrar permisos de usuario**.</span><span class="sxs-lookup"><span data-stu-id="28d77-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="28d77-109">Agregue usuarios que necesiten permisos para crear su sitio de Mis sitios.</span><span class="sxs-lookup"><span data-stu-id="28d77-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="28d77-110">De forma predeterminada, esta configuración se establece en **Todos excepto los usuarios externos.**</span><span class="sxs-lookup"><span data-stu-id="28d77-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="28d77-111">Después de agregar el usuario, los usuarios o el grupo, asegúrese de que el usuario, los usuarios o el grupo agregados están **seleccionados,** desplácese a la sección de permisos y, a continuación, active la casilla junto a Crear sitio **personal (necesario** para el almacenamiento personal, el servicio de noticias y el contenido seguido).</span><span class="sxs-lookup"><span data-stu-id="28d77-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="28d77-112">Haga **clic en** Aceptar y, a continuación, haga que el usuario vaya a la página de OneDrive para crear el sitio.</span><span class="sxs-lookup"><span data-stu-id="28d77-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
