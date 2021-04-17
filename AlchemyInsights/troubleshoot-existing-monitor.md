---
title: Solución de problemas del monitor existente
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824596"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="acb8b-102">Solucionar problemas de un monitor existente</span><span class="sxs-lookup"><span data-stu-id="acb8b-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="acb8b-103">Pruebe estas soluciones para solucionar problemas de un monitor.</span><span class="sxs-lookup"><span data-stu-id="acb8b-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="acb8b-104">**Actualice la pantalla del monitor:**</span><span class="sxs-lookup"><span data-stu-id="acb8b-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="acb8b-105">Presione las siguientes teclas al mismo tiempo: Tecla Windows + Ctrl + Mayús + B. Esto actualizará la comunicación con el controlador de gráficos.</span><span class="sxs-lookup"><span data-stu-id="acb8b-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="acb8b-106">Los monitores parpadearán momentáneamente y volverán después de unos segundos.</span><span class="sxs-lookup"><span data-stu-id="acb8b-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="acb8b-107">**Solucionar problemas de hardware de monitor:**</span><span class="sxs-lookup"><span data-stu-id="acb8b-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="acb8b-108">Desconecte el cable que conecta el PC al monitor y vuelva a conectarlo.</span><span class="sxs-lookup"><span data-stu-id="acb8b-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="acb8b-109">Desconecte los dispositivos no esenciales del PC (como adaptadores o docks).</span><span class="sxs-lookup"><span data-stu-id="acb8b-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="acb8b-110">**Si has instalado recientemente una actualización en el equipo, puedes revertir el controlador de pantalla:**</span><span class="sxs-lookup"><span data-stu-id="acb8b-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="acb8b-111">Selecciona **Inicio**, escribe **Administrador de** dispositivos y selecciona Administrador de **dispositivos** en los resultados.</span><span class="sxs-lookup"><span data-stu-id="acb8b-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="acb8b-112">Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Propiedades**.</span><span class="sxs-lookup"><span data-stu-id="acb8b-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="acb8b-113">Vaya a la **pestaña Controlador** y seleccione **Revertir controlador**.</span><span class="sxs-lookup"><span data-stu-id="acb8b-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="acb8b-114">Nota: Si no está disponible o está atenuado, seleccione **No** en las opciones siguientes para pasar al siguiente paso.</span><span class="sxs-lookup"><span data-stu-id="acb8b-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="acb8b-115">Es posible que deba reiniciar el equipo antes de que estos cambios sumen efecto.</span><span class="sxs-lookup"><span data-stu-id="acb8b-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="acb8b-116">**Desinstale y vuelva a instalar el controlador de pantalla:**</span><span class="sxs-lookup"><span data-stu-id="acb8b-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="acb8b-117">Selecciona **Inicio**, escribe **Administrador de** dispositivos y selecciona Administrador de **dispositivos** en los resultados.</span><span class="sxs-lookup"><span data-stu-id="acb8b-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="acb8b-118">Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Desinstalar dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="acb8b-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="acb8b-119">Seleccione el cuadro situado junto **a Eliminar el software del controlador para este dispositivo** y seleccione **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="acb8b-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="acb8b-120">Nota: Es posible que se te pida que reinicies el equipo en esta fase.</span><span class="sxs-lookup"><span data-stu-id="acb8b-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="acb8b-121">Asegúrese de escribir las instrucciones restantes antes de reiniciar.</span><span class="sxs-lookup"><span data-stu-id="acb8b-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="acb8b-122">Abre el Administrador de dispositivos de nuevo.</span><span class="sxs-lookup"><span data-stu-id="acb8b-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="acb8b-123">Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Actualizar controlador**.</span><span class="sxs-lookup"><span data-stu-id="acb8b-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="acb8b-124">Seleccione **Buscar automáticamente el software del controlador de actualización** y siga las instrucciones de instalación.</span><span class="sxs-lookup"><span data-stu-id="acb8b-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>