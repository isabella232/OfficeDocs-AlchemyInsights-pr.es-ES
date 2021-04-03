---
title: Liberar espacio en disco en Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505373"
---
# <a name="free-up-drive-space-in-windows-10"></a>Liberar espacio en disco en Windows 10

Estas son las dos opciones para liberar espacio en disco en Windows:

- Liberar espacio en disco en Windows 10.
- Liberar espacio para las actualizaciones de Windows 10 con dispositivo de almacenamiento externo.

Si todavía tiene poco espacio en disco después de usar el Liberador de espacio en disco, es posible que la carpeta Temp se esté llenando rápidamente con archivos de aplicación (.appx) usados por Microsoft Store. Para solucionar este problema, restablezca la Store, borre la caché de Store y ejecute el solucionador de problemas de Windows Update. Asegúrese de que Microsoft Store está cerrado antes de continuar con estos pasos.

**Paso 1: Restablecer Microsoft Store**

**Nota** Esta acción elimina de forma permanente los datos de la aplicación en el dispositivo, incluidos sus preferencias y detalles de inicio de sesión.

1. Seleccione **Inicio** > **Configuración** > **Aplicaciones** > **Aplicaciones y características**.

1. En la lista de aplicaciones, busque y seleccione Microsoft Store.

1. Seleccione **Opciones avanzadas**.

1. Desplácese hacia abajo y seleccione **Restablecer** y, después, **Confirmar restablecimiento**.

**Paso 2: Borrar la caché de Microsoft Store**

1. Pulse la tecla del logotipo de Windows + R para abrir el cuadro de diálogo Ejecutar.

1. Escriba wsreset.exe y seleccione **Aceptar**.

1. Se abrirá una ventana del símbolo del sistema en blanco. Después de unos 10 segundos, se cerrará la ventana y la Store se abrirá automáticamente.

**Paso 3: Restablecer Windows Update**

1. Seleccione **Inicio** > **Configuración** > **Actualización y seguridad** > **Solución de problemas**.

1. Desplácese hacia abajo y seleccione **Windows Update** de la lista y, después, **Ejecute el solucionador de problemas**.

1. Reinicie el equipo y compruebe si todavía está experimentando el problema.

