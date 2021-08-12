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
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939900"
---
# <a name="troubleshoot-access-denied-messages"></a>Solucionar problemas de acceso denegado

Si alguien recibió un mensaje "Acceso denegado" a una carpeta compartida en SharePoint, el administrador de la colección de sitios podría haber habilitado "Modo de bloqueo de permisos de usuario de acceso limitado". Para desactivar esto: 
  
1. Vaya al sitio, haga clic en el icono Configuración y, a continuación, haga clic en **Sitio Configuración**.
    
2. En **Administración de la colección de sitios**, haga clic en **Características de la colección de sitios**.
    
3. Junto al modo de bloqueo de permisos de usuario de acceso **limitado,** haga clic **en Desactivar**.
    
También se puede producir un mensaje de acceso denegado para carpetas compartidas si el sitio es un sitio de publicación. Para obtener información, consulta [Acceso denegado al acceder a una carpeta compartida.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Si alguien recibió un mensaje de "Acceso denegado" al intentar ver solicitudes de acceso, el usuario debe agregarse como administrador de la colección de sitios o como miembro del grupo Propietarios del sitio. Para obtener más información, [consulta Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Si un usuario recibió un mensaje de "Acceso denegado" después de que se quitaron de Active Directory local y, a continuación, se agregaron de nuevo, vea [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

