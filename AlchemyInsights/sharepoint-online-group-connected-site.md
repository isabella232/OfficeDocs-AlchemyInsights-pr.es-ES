---
title: Agregar un grupo a un SharePoint sitio
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532236"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemas comunes al crear un sitio conectado a un grupo en SharePoint

1. Si ha eliminado un grupo y su sitio conectado y desea crear otro sitio con la misma dirección URL, deberá quitar permanentemente el sitio anterior.

   - Descargar [shell de administración de SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Para obtener más información sobre cómo empezar a usar Powershell, consulta [Introducción a SharePoint Shell de administración en línea](/powershell/module/sharepoint-online/remove-sposite).
   - Quite el sitio de sitios eliminados mediante el cmdlet [Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell es necesario para eliminar permanentemente sitios de grupo.

1. Si está creando un sitio conectado a un grupo y recibe una advertencia: ya existe otro grupo con el mismo **alias,** compruebe los grupos existentes desde [el Centro de administración de Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Para resolver el problema, elimine el grupo existente si ya no es necesario o cree el sitio con un alias diferente asignado.

1. Hay diferentes formas de crear y usar grupos modernos con SharePoint.

   - Puede conectar sitios existentes a un Microsoft 365 grupo. Para obtener más información, [consulta Conectar un grupo Microsoft 365 mediante la interfaz SharePoint usuario](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Para crear un Microsoft 365 de grupo conectado, deberá crear un sitio [de grupo](https://admin.microsoft.com/sharepoint).
