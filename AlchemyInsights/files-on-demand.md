---
title: Archivos a petición
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745305"
---
# <a name="configure-files-on-demand"></a>Configurar Archivos a petición

Archivos a petición de OneDrive permite tener acceso a todos los archivos en OneDrive sin necesidad de descargarlos todos ni usar espacio de almacenamiento en el dispositivo.

Para configurar Archivos a petición en su PC:

1. Seleccione el icono de nube de color blanco o azul de **OneDrive** en el área de notificaciones de la barra de tareas de Windows. Seleccione el icono de engranaje de **Ayuda y configuración** > **Configuración**.
2. En la pestaña **Configuración**, seleccione la casilla **Ahorrar espacio y descargar archivos a medida que se usan**.  

También puede configurar Archivos a petición con el registro.

Si usted deshabilita esta configuración, los usuarios de Windows 10 tienen el mismo comportamiento de sincronización que tienen los usuarios de versiones anteriores de Windows y no pueden activar los archivos a pedido. Si no configura esta opción, los usuarios pueden activar o desactivar Archivos a petición.

Si habilita esta directiva, el valor de la siguiente clave del Registro se establece en “1”. Si deshabilita esta directiva, el valor de la siguiente clave del registro se establece en 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Si no puede ver la opción de Archivos a petición en "Configuración", asegúrese de que el tipo de inicio del servicio "Controlador de filtro de archivos de la nube de Windows" está establecido en 2 (AUTO_START). Si habilita esta característica, el valor de la siguiente clave de registro se establece en 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`