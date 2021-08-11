---
title: Configuración de inicio en Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909843"
---
# <a name="startup-settings-in-windows-10"></a>Configuración de inicio en Windows 10

**Cambiar las aplicaciones que se ejecutan automáticamente al inicio**

1. Vaya a [Configuración > Aplicaciones > Inicio.](ms-settings:startupapps?activationSource=GetHelp)

2. Asegúrate de que cualquier aplicación que quieras ejecutar en el inicio esté **activada**.

**Agregar una aplicación para que se ejecute automáticamente al inicio**

1. Haz clic o pulsa **en Inicio** y busca la aplicación que quieres ejecutar al inicio.

2. Haga clic con el botón secundario en la aplicación, haga clic en **Más** y, a continuación, haga clic **en Abrir ubicación del archivo**. Se abre la ubicación donde se guarda el acceso directo a la aplicación. Si no hay ninguna opción para la ubicación de abrir archivo, significa que la aplicación no se puede ejecutar al inicio.

3. Con la ubicación del archivo abierta, presione la tecla **Windows logotipo + R**, escriba **shell:startup** y, a continuación, haga clic en **Aceptar**. Se abre la carpeta Inicio.

4. Copie y pegue el acceso directo a la aplicación desde la ubicación del archivo a la carpeta Inicio.

**Opciones avanzadas de inicio (incluido el Caja fuerte, la configuración de UEFI y el arranque desde otro dispositivo)**

1. Guarde el trabajo y cierre los documentos abiertos, ya que estos pasos reiniciarán el equipo.

2. Vaya a [Configuración > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. En **Inicio avanzado,** haga clic **en Reiniciar ahora**. 

4. Después de reiniciar el equipo en la pantalla elegir una opción:

    - Para arrancar desde un dispositivo como una unidad USB, haga clic **en Usar un dispositivo**.

    - Para especificar la configuración de UEFI (a veces denominada configuración del BIOS), haga clic en Solucionar problemas > opciones avanzadas > **uefi firmware Configuración**. 

    - Para escribir el modo Caja fuerte o cambiar la configuración de inicio avanzada, haga clic en Solucionar problemas > opciones avanzadas > **inicio Configuración** y, a continuación, haga clic en **Reiniciar**. Es posible que se te pida que escribas la [clave de recuperación de BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Después de reiniciar de nuevo el equipo, haz clic en la configuración de inicio que quieras usar.