---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830599"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="d7ab8-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="d7ab8-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="d7ab8-103">¿Trabaja con PowerShell o scripts en Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="d7ab8-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="d7ab8-104">Visite los vínculos siguientes para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="d7ab8-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="d7ab8-105">Introducción al Shell de administración de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d7ab8-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="d7ab8-106">Conectarse a PowerShell de SPO con autenticación multifactor (MFA)</span><span class="sxs-lookup"><span data-stu-id="d7ab8-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="d7ab8-107">[Patrones y prácticas de SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiene una biblioteca de comandos de PowerShell que le permite realizar acciones de administración complejas hacia SPO.</span><span class="sxs-lookup"><span data-stu-id="d7ab8-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="d7ab8-108">Si tiene problemas para conectarse con el shell de administración de SPO, asegúrese de que se ha actualizado a la versión más reciente e intente [volver](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) a importar el módulo con *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="d7ab8-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="d7ab8-109">Si está intentando ejecutar scripts del modelo de objetos del lado cliente, tendrá que tener instalado el SDK de componentes de cliente de [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) en el equipo local.</span><span class="sxs-lookup"><span data-stu-id="d7ab8-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="d7ab8-110">Si tiene problemas para ejecutar scripts desde PowerShell, es posible que desee considerar la posibilidad de ejecutar PowerShell como administrador y cambiar la [directiva de ejecución.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="d7ab8-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>