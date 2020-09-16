---
title: PowerShell de SharePoint Online
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770856"
---
# <a name="sharepoint-online-powershell"></a>PowerShell de SharePoint Online

¿Trabaja con PowerShell o scripts en SharePoint Online? Visite los siguientes vínculos para obtener más información.
- [Introducción al Shell de administración de SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Conectarse a la PowerShell de SPO con la autenticación multifactor (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Modelos y prácticas de SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiene una biblioteca de comandos de PowerShell que le permite realizar acciones de administración complejas en SPO.

> [!NOTE]
> - Si tiene problemas para conectarse con el shell de administración de SPO, asegúrese de que se ha actualizado a la versión más reciente e intente [volver a importar el módulo](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) mediante *"Import-Module Microsoft. online. SharePoint. PowerShell".*
> - Si está intentando ejecutar scripts de modelo de objetos del lado cliente, deberá tener instalado el [SDK de componentes de cliente de SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) en el equipo local.
> - Si tiene problemas al ejecutar scripts de PowerShell, es posible que desee considerar la posibilidad de ejecutar PowerShell como administrador y cambiar la [Directiva de ejecución](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).