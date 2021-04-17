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
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

¿Trabaja con PowerShell o scripts en Sharepoint Online? Visite los vínculos siguientes para obtener más información.
- [Introducción al Shell de administración de SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Conectarse a PowerShell de SPO con autenticación multifactor (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Patrones y prácticas de SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiene una biblioteca de comandos de PowerShell que le permite realizar acciones de administración complejas hacia SPO.

> [!NOTE]
> - Si tiene problemas para conectarse con el shell de administración de SPO, asegúrese de que se ha actualizado a la versión más reciente e intente [volver](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) a importar el módulo con *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Si está intentando ejecutar scripts del modelo de objetos del lado cliente, tendrá que tener instalado el SDK de componentes de cliente de [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) en el equipo local.
> - Si tiene problemas para ejecutar scripts desde PowerShell, es posible que desee considerar la posibilidad de ejecutar PowerShell como administrador y cambiar la [directiva de ejecución.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)