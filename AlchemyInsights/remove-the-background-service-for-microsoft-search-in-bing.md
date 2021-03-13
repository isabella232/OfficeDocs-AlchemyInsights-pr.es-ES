---
title: Quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753444"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="abacb-102">Quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing</span><span class="sxs-lookup"><span data-stu-id="abacb-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="abacb-103">Para quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing, puede probar lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="abacb-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="abacb-104">Para revertir a la configuración original del motor de búsqueda, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="abacb-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="abacb-105">a.</span><span class="sxs-lookup"><span data-stu-id="abacb-105">a.</span></span> <span data-ttu-id="abacb-106">Desactive el **botón de alternancia[ de](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)Usar Bing como motor de búsqueda predeterminado**.</span><span class="sxs-lookup"><span data-stu-id="abacb-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="abacb-107">b.</span><span class="sxs-lookup"><span data-stu-id="abacb-107">b.</span></span> <span data-ttu-id="abacb-108">[Vaya al Centro de administración de Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) y elimine la configuración que afecta a todos los usuarios de su organización.</span><span class="sxs-lookup"><span data-stu-id="abacb-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="abacb-109">Para quitar el servicio en segundo plano de un dispositivo individual, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="abacb-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="abacb-110">a.</span><span class="sxs-lookup"><span data-stu-id="abacb-110">a.</span></span> <span data-ttu-id="abacb-111">Elija **Panel de control > Programas > Programas y características**.</span><span class="sxs-lookup"><span data-stu-id="abacb-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="abacb-112">b.</span><span class="sxs-lookup"><span data-stu-id="abacb-112">b.</span></span> <span data-ttu-id="abacb-113">Haga clic con el botón derecho en **Búsqueda de Microsoft en Bing** en la lista de programas instalados, y haga clic en **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="abacb-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="abacb-114">Para quitar el servicio en segundo plano de varios dispositivos en su organización, inicie sesión como administrador y ejecute el siguiente comando en un script:</span><span class="sxs-lookup"><span data-stu-id="abacb-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
