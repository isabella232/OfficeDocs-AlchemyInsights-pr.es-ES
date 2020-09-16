---
title: Problemas de conexión de SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727188"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemas de conexión de SharePoint Designer 

Si SharePoint Designer tiene problemas de conexión con los sitios de SharePoint, pruebe las siguientes soluciones comunes.

Paso 1: comprobar que SharePoint Designer 2013 se ha actualizado con [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) y la [actualización de 2 de agosto de 2016 para SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Paso 2: borrar los archivos de la caché local:

1. Cierre SharePoint Designer 2013.

2. En el equipo local, quite todos los archivos que se encuentren en cada una de las carpetas siguientes.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra SharePoint Designer 2013 y vuelva a escribir la cuenta para ver si funciona.

Paso 3: [Habilitar la autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Paso 4: los administradores deberán permitir el **script personalizado** en la configuración del centro de administración de SharePoint para permitir la conexión de SharePoint Designer. Consulte [permitir o impedir el script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obtener más información.


