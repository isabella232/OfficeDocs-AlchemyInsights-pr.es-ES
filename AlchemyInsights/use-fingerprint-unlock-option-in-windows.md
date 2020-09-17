---
title: Usar la opción de desbloqueo de huellas digitales en Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795261"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="d3abc-102">Usar la opción de desbloqueo de huellas digitales en Windows 10</span><span class="sxs-lookup"><span data-stu-id="d3abc-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="d3abc-103">**Habilitar huella digital de Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="d3abc-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="d3abc-104">Para desbloquear Windows 10 con tu huella digital, debes configurar la huella digital de Windows Hello agregando (permitiendo que Windows aprenda a reconocer), al menos, un dedo.</span><span class="sxs-lookup"><span data-stu-id="d3abc-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="d3abc-105">Vaya a **configuración > cuentas > opciones de inicio de sesión** (o haga clic [aquí](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="d3abc-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d3abc-106">Se mostrarán las opciones de inicio de sesión disponibles.</span><span class="sxs-lookup"><span data-stu-id="d3abc-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="d3abc-107">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="d3abc-107">For example:</span></span>

    ![Opciones de inicio de sesión.](media/sign-in-options.png)

2. <span data-ttu-id="d3abc-109">Haga clic o pulse **huella digital de Windows Hello**y, a continuación, haga clic en **configurar**.</span><span class="sxs-lookup"><span data-stu-id="d3abc-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="d3abc-110">En la ventana de configuración de Windows Hello **, haga clic en introducción.**</span><span class="sxs-lookup"><span data-stu-id="d3abc-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="d3abc-111">El sensor de huellas digitales se activará y se le pedirá que ponga el dedo en el sensor:</span><span class="sxs-lookup"><span data-stu-id="d3abc-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor de huellas digitales.](media/fingerprint-sensor.png)

3. <span data-ttu-id="d3abc-113">Sigue las instrucciones, que te pedirán que digitalices el dedo repetidamente.</span><span class="sxs-lookup"><span data-stu-id="d3abc-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="d3abc-114">Cuando termine, tendrá la opción de agregar otros dedos que quiera usar para el inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="d3abc-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="d3abc-115">La próxima vez que inicie sesión en Windows 10, tendrá la opción de usar su huella dactilar para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="d3abc-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="d3abc-116">**Huella digital de Windows Hello no disponible como opción de inicio de sesión**</span><span class="sxs-lookup"><span data-stu-id="d3abc-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="d3abc-117">Si la huella digital de Windows Hello no se muestra como una opción en **Opciones de inicio de sesión**, significa que Windows no tiene constancia de ningún escáner o lector de huellas digitales conectado a tu PC, o que una directiva del sistema impide su uso (si, por ejemplo, el equipo está administrado por el área de trabajo).</span><span class="sxs-lookup"><span data-stu-id="d3abc-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="d3abc-118">Para solucionar problemas:</span><span class="sxs-lookup"><span data-stu-id="d3abc-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="d3abc-119">Seleccione el botón **Inicio** de la barra de tareas y busque **Administrador de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="d3abc-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="d3abc-120">Haga clic o pulse para abrir el **Administrador de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="d3abc-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="d3abc-121">En el administrador de dispositivos, expanda dispositivos biométricos haciendo clic en su cheurón.</span><span class="sxs-lookup"><span data-stu-id="d3abc-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. <span data-ttu-id="d3abc-123">El escáner de huellas digitales debe aparecer como un dispositivo biométrico, como el explorador de WBDI de Synaptics:</span><span class="sxs-lookup"><span data-stu-id="d3abc-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="d3abc-125">Si no se muestra el escáner de huellas digitales y el escáner está integrado en el equipo, ve al sitio web del fabricante del equipo.</span><span class="sxs-lookup"><span data-stu-id="d3abc-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="d3abc-126">En la sección de soporte técnico de su modelo de equipo, busque un controlador de Windows 10 para un escáner que pueda instalar.</span><span class="sxs-lookup"><span data-stu-id="d3abc-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="d3abc-127">Si el escáner es independiente del equipo (conectado a través de USB), ve al sitio web del fabricante del escáner para buscar e instalar el software de controlador de dispositivo de Windows 10 para el modelo de escáner que tienes.</span><span class="sxs-lookup"><span data-stu-id="d3abc-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
