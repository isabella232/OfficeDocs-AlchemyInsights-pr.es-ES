---
title: Solucionar problemas de mensajes de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690800"
---
# <a name="troubleshoot-access-denied-messages"></a>Solucionar problemas de mensajes de acceso denegado

Si alguien recibe un mensaje "acceso denegado" a una carpeta compartida de SharePoint, es posible que el administrador de la colección de sitios haya habilitado el modo de bloqueo de permisos de usuario de acceso limitado. Para desactivarlo: 
  
1. Vaya al sitio, haga clic en el icono configuración y, a continuación, haga clic en **configuración del sitio**.
    
2. En **Administración de la colección de sitios**, haga clic en **Características de la colección de sitios**.
    
3. Junto a **modo de bloqueo de permisos de usuario de acceso limitado**, haga clic en **desactivar**.
    
Un mensaje de acceso denegado también puede producirse para carpetas compartidas si el sitio es un sitio de publicación. Para obtener información, vea [acceso denegado cuando se tiene acceso a una carpeta compartida](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Si un usuario obtuvo un mensaje de "acceso denegado" al intentar ver las solicitudes de acceso, el usuario debe agregarse como administrador de la colección de sitios o como miembro del grupo de propietarios del sitio. Para obtener más información, consulte [acceso denegado a solicitudes de acceso a la lista de solicitudes](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Si un usuario obtuvo un mensaje de "acceso denegado" después de que se quitó de Active Directory local y después se volvió a agregar, vea [acceso denegado cuando una cuenta de usuario se sincroniza con Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

