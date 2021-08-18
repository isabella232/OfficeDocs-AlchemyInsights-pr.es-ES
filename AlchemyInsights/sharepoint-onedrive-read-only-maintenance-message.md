---
title: Read-Only mensaje de mantenimiento al intentar usar SharePoint o OneDrive
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
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329465"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only mensaje de mantenimiento al intentar usar SharePoint o OneDrive

Los usuarios pueden recibir un **mensaje de solo** lectura para mantenimiento al intentar usar SharePoint o OneDrive para uno de los siguientes escenarios. 

-   Una actividad de mantenimiento planeada o activa.  Para comprobarlos, vaya al Centro [de mensajes](https://portal.office.com/adminportal/home#/messagecenter).
-   Un incidente de servicio activo de alta prioridad que puede estar ocurriendo. Compruebe si hay avisos o incidentes navegando a [Estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).
-   Un escenario de recuperación de recuperación automática menor que podría estar ocurriendo debido a eventos inesperados en los servidores que podrían durar menos de 30 minutos. 
    
    No hay publicaciones del centro de mensajes ni del estado del servicio para estas recuperaciones secundarias, pero debe volver a la normalidad muy pronto.

En muy pocas ocasiones, observamos que uno de los tres escenarios enumerados anteriormente ha sido la causa y el servicio se ha restaurado, pero la memoria caché del explorador de los usuarios no se ha aclarado.

Intente borrar la memoria caché del explorador antes de navegar al sitio.

1. En el Microsoft Edge, seleccione **Configuración** y, a continuación, **seleccione Privacidad y seguridad**.
2. En **Borrar exploración,** **seleccione Elegir qué borrar**.
3. Seleccione **Cookies y datos del sitio web guardados** y seleccione **Borrar**.

**Nota:** Estos pasos pueden diferir al usar otros exploradores como Mozilla Firefox o Google Chrome.

**Nota:** Otra opción sería abrir el sitio SharePoint o OneDrive en una nueva ventana de InPrivate.