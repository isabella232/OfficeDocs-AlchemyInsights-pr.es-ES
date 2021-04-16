---
title: El icono de batería o de energía no se encuentra en Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790565"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>El icono de batería o de energía no se encuentra en Windows 10

Si su dispositivo con Windows 10 tiene una batería (por ejemplo, un portátil o tableta, o un equipo conectado mediante USB a un sistema de alimentación ininterrumpida), normalmente se mostrará un icono de batería o de energía en la barra de tareas cerca del reloj, por ejemplo:

![Icono de batería](media/battery-icon.png)

Si no ve este icono, es posible que esté oculto:

1. Vaya a **[Configuración > Personalización > Barra de tareas](ms-settings:taskbar?activationSource=GetHelp)**.

2. En el área de Notificaciones, haga clic en **Seleccionar los iconos que aparecerán en la barra de tareas**.

3. Después, busque en la lista el elemento **Energía** y cambie el valor a **Activado**.

    ![Mostrar el icono de energía en la barra de tareas](media/power-icon-on.png)

**Solución de problemas**

Si ha seguido las instrucciones anteriores y el botón de alternancia **Energía** se muestra atenuado o no visible, en el cuadro de búsqueda de la barra de tareas, escriba **Administrar dispositivos** y seleccione **Administrador de dispositivos** en la lista de resultados. En **Baterías**, haga clic con el botón derecho en la batería del dispositivo, haga clic en **Deshabilitar** y haga clic en **Sí**. Espere unos segundos y haga clic con el botón derecho en la batería y haga clic en **Habilitar**. Después reinicie el dispositivo.

Si ha seguido las instrucciones anteriores, pero el icono de batería no aparece en la barra de tareas, en el cuadro de búsqueda de la barra de tareas, escriba **Administrador de tareas** y haga clic en **Administrador de tareas** en la lista de resultados. En la pestaña **Procesos**, en **Nombre**, haga clic con el botón derecho en **Explorador** y haga clic en **Reiniciar**.  
