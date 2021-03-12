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
# <a name="troubleshoot-access-denied-messages"></a>Solucionar problemas de acceso denegado

Si alguien recibió un mensaje "Acceso denegado" a una carpeta compartida en SharePoint, es posible que el administrador de la colección de sitios haya habilitado "Modo de bloqueo de permisos de usuario de acceso limitado". Para desactivar esto: 
  
1. Vaya al sitio, haga clic en el icono Configuración y, a continuación, haga clic en **Configuración del sitio**.
    
2. En **Administración de la colección de sitios**, haga clic en **Características de la colección de sitios**.
    
3. Junto al modo de bloqueo de permisos de usuario de acceso **limitado,** haga clic **en Desactivar**.
    
También se puede producir un mensaje de acceso denegado para carpetas compartidas si el sitio es un sitio de publicación. Para obtener información, consulta [Acceso denegado al acceder a una carpeta compartida.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Si alguien recibió un mensaje de "Acceso denegado" al intentar ver solicitudes de acceso, el usuario debe agregarse como administrador de la colección de sitios o como miembro del grupo Propietarios del sitio. Para obtener más información, [consulta Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Si un usuario recibió un mensaje de "Acceso denegado" después de que se quitara de Active Directory localmente y, a continuación, se agregara de nuevo, vea [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

