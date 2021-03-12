---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709087"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fa5ba-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fa5ba-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fa5ba-103">¿Trabaja con PowerShell o scripts en Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="fa5ba-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fa5ba-104">Visite los vínculos siguientes para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="fa5ba-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fa5ba-105">Introducción al Shell de administración de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fa5ba-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fa5ba-106">Conectarse a PowerShell de SPO con autenticación multifactor (MFA)</span><span class="sxs-lookup"><span data-stu-id="fa5ba-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fa5ba-107">[Patrones y prácticas de SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiene una biblioteca de comandos de PowerShell que le permite realizar acciones de administración complejas hacia SPO.</span><span class="sxs-lookup"><span data-stu-id="fa5ba-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fa5ba-108">Si tiene problemas para conectarse con el shell de administración de SPO, asegúrese de que se ha actualizado a la versión más reciente e intente [volver](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) a importar el módulo con *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="fa5ba-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fa5ba-109">Si está intentando ejecutar scripts del modelo de objetos del lado cliente, tendrá que tener instalado el SDK de componentes de cliente de [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) en el equipo local.</span><span class="sxs-lookup"><span data-stu-id="fa5ba-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fa5ba-110">Si tiene problemas para ejecutar scripts desde PowerShell, es posible que desee considerar la posibilidad de ejecutar PowerShell como administrador y cambiar la [directiva de ejecución.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="fa5ba-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>