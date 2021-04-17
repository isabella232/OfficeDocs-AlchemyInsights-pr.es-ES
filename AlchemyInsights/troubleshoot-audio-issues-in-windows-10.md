---
title: Solucionar problemas de audio en Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833308"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="fcd2c-102">Solución de problemas de audio en Windows 10</span><span class="sxs-lookup"><span data-stu-id="fcd2c-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="fcd2c-103">**Ejecutar el solucionador de problemas de audio**</span><span class="sxs-lookup"><span data-stu-id="fcd2c-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="fcd2c-104">Abra la configuración [de solución de problemas](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="fcd2c-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="fcd2c-105">Seleccione **Reproducir audio** Ejecute el  >  **solucionador de problemas**.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="fcd2c-106">**Establecer el dispositivo predeterminado**</span><span class="sxs-lookup"><span data-stu-id="fcd2c-106">**Set the default device**</span></span>

<span data-ttu-id="fcd2c-107">Si te conectas a un dispositivo de audio con USB o HDMI, es posible que debas establecer ese dispositivo como predeterminado:</span><span class="sxs-lookup"><span data-stu-id="fcd2c-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="fcd2c-108">Abra **Iniciar**  >  **sonido** y, a continuación, seleccione **Sonido** o **Cambiar sonidos** del sistema en la lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="fcd2c-109">En la **pestaña Reproducción,** seleccione un dispositivo, **seleccione Establecer predeterminado** y, a continuación, seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="fcd2c-110">**Comprobar cables, volumen, altavoces y auriculares**</span><span class="sxs-lookup"><span data-stu-id="fcd2c-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="fcd2c-111">Compruebe si hay cables sueltos en las conexiones de altavoces y auriculares y asegúrese de que están conectados al conector correcto.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="fcd2c-112">Comprueba los niveles de energía y volumen e intenta activar todos los controles de volumen.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="fcd2c-113">Algunos altavoces y aplicaciones tienen sus propios controles de volumen; es posible que deba comprobarlos todos para asegurarse de que están en los niveles correctos.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="fcd2c-114">Intente conectarse con un puerto USB diferente.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="fcd2c-115">**Nota:** Recuerde que es posible que los altavoces no funcionen cuando los auriculares están conectados.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="fcd2c-116">**Comprobar administrador de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="fcd2c-116">**Check Device Manager**</span></span>

<span data-ttu-id="fcd2c-117">Para asegurarse de que los controladores están actualizados:</span><span class="sxs-lookup"><span data-stu-id="fcd2c-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="fcd2c-118">Selecciona **Inicio**, escribe **Administrador de** dispositivos y, a continuación, selecciona Administrador **de** dispositivos en la lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="fcd2c-119">En **Controladores de sonido, vídeo** y juegos, selecciona tu tarjeta de sonido, ábrala, selecciona la pestaña Controlador y selecciona Actualizar **controlador**. </span><span class="sxs-lookup"><span data-stu-id="fcd2c-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="fcd2c-120">**Nota:** Si Windows no encuentra un controlador nuevo, busca uno en el sitio web del fabricante del dispositivo y sigue sus instrucciones.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="fcd2c-121">**Reinstalar el controlador**</span><span class="sxs-lookup"><span data-stu-id="fcd2c-121">**Reinstall the driver**</span></span>

<span data-ttu-id="fcd2c-122">Si no puedes actualizar a través del Administrador de dispositivos o encontrar un nuevo controlador en el sitio web del fabricante, prueba estos pasos:</span><span class="sxs-lookup"><span data-stu-id="fcd2c-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="fcd2c-123">En el Administrador de dispositivos, haga clic con el botón secundario (o mantenga presionado) el controlador de audio y seleccione **Desinstalar**.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="fcd2c-124">Reinicia el dispositivo y Windows intentará reinstalar el controlador.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="fcd2c-125">Si reinstalar el controlador no funciona, prueba a usar el controlador de audio genérico que viene con Windows.</span><span class="sxs-lookup"><span data-stu-id="fcd2c-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="fcd2c-126">En el Administrador de dispositivos, haga clic con el botón secundario (o presione y mantenga presionado) el **controlador** de audio > Actualizar software del controlador Examinar mi equipo en busca de software de controladores Permítanme elegir de una lista de controladores de dispositivo en mi equipo , seleccione Dispositivo de audio de alta definición, seleccione Siguiente y siga las instrucciones para  >    >  instalarlo.  </span><span class="sxs-lookup"><span data-stu-id="fcd2c-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
