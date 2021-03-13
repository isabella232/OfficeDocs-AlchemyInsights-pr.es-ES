---
title: Quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753444"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing

Para quitar el servicio en segundo plano para la Búsqueda de Microsoft en Bing, puede probar lo siguiente:

1. Para revertir a la configuración original del motor de búsqueda, haga lo siguiente:

    a. Desactive el **botón de alternancia[ de](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)Usar Bing como motor de búsqueda predeterminado**.

    b. [Vaya al Centro de administración de Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) y elimine la configuración que afecta a todos los usuarios de su organización.

2. Para quitar el servicio en segundo plano de un dispositivo individual, haga lo siguiente:

    a. Elija **Panel de control > Programas > Programas y características**.

    b. Haga clic con el botón derecho en **Búsqueda de Microsoft en Bing** en la lista de programas instalados, y haga clic en **Desinstalar**.

3. Para quitar el servicio en segundo plano de varios dispositivos en su organización, inicie sesión como administrador y ejecute el siguiente comando en un script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
