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
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="532a9-102">El icono de batería o de energía no se encuentra en Windows 10</span><span class="sxs-lookup"><span data-stu-id="532a9-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="532a9-103">Si su dispositivo con Windows 10 tiene una batería (por ejemplo, un portátil o tableta, o un equipo conectado mediante USB a un sistema de alimentación ininterrumpida), normalmente se mostrará un icono de batería o de energía en la barra de tareas cerca del reloj, por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="532a9-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Icono de batería](media/battery-icon.png)

<span data-ttu-id="532a9-105">Si no ve este icono, es posible que esté oculto:</span><span class="sxs-lookup"><span data-stu-id="532a9-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="532a9-106">Vaya a **[Configuración > Personalización > Barra de tareas](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="532a9-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="532a9-107">En el área de Notificaciones, haga clic en **Seleccionar los iconos que aparecerán en la barra de tareas**.</span><span class="sxs-lookup"><span data-stu-id="532a9-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="532a9-108">Después, busque en la lista el elemento **Energía** y cambie el valor a **Activado**.</span><span class="sxs-lookup"><span data-stu-id="532a9-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Mostrar el icono de energía en la barra de tareas](media/power-icon-on.png)

<span data-ttu-id="532a9-110">**Solución de problemas**</span><span class="sxs-lookup"><span data-stu-id="532a9-110">**Troubleshooting**</span></span>

<span data-ttu-id="532a9-111">Si ha seguido las instrucciones anteriores y el botón de alternancia **Energía** se muestra atenuado o no visible, en el cuadro de búsqueda de la barra de tareas, escriba **Administrar dispositivos** y seleccione **Administrador de dispositivos** en la lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="532a9-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="532a9-112">En **Baterías**, haga clic con el botón derecho en la batería del dispositivo, haga clic en **Deshabilitar** y haga clic en **Sí**.</span><span class="sxs-lookup"><span data-stu-id="532a9-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="532a9-113">Espere unos segundos y haga clic con el botón derecho en la batería y haga clic en **Habilitar**.</span><span class="sxs-lookup"><span data-stu-id="532a9-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="532a9-114">Después reinicie el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="532a9-114">Then restart your device.</span></span>

<span data-ttu-id="532a9-115">Si ha seguido las instrucciones anteriores, pero el icono de batería no aparece en la barra de tareas, en el cuadro de búsqueda de la barra de tareas, escriba **Administrador de tareas** y haga clic en **Administrador de tareas** en la lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="532a9-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="532a9-116">En la pestaña **Procesos**, en **Nombre**, haga clic con el botón derecho en **Explorador** y haga clic en **Reiniciar**.  </span><span class="sxs-lookup"><span data-stu-id="532a9-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
