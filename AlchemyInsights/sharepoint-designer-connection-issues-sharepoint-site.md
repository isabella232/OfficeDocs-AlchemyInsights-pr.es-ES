---
title: SharePoint Problemas de conexión del diseñador
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942042"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemas de conexión del diseñador 

Si SharePoint Designer está experimentando problemas de conexión a SharePoint, pruebe las siguientes soluciones comunes.

Paso [1:](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) Comprobar que SharePoint Designer 2013 se actualiza con SharePoint Designer Service Pack 1 y la actualización del 2 de agosto de [2016 para SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Paso 2: Borrar los archivos de caché local:

1. Cierre SharePoint Designer 2013.

2. En el equipo local, quite todos los archivos encontrados en cada una de las carpetas siguientes.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Abra SharePoint Designer 2013 y vuelva a escribir la cuenta para ver si funciona.

Paso 3: [Habilitar la autenticación moderna para Office 2013 en Windows dispositivos](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Paso 4: Los administradores tendrán que permitir **script** personalizado en la configuración del Centro de administración de SharePoint para permitir la conexión SharePoint Designer. Vea [Permitir o impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) para obtener más información.


