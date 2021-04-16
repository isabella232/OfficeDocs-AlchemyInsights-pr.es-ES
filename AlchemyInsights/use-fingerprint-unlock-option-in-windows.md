---
title: Usar la opción de desbloqueo de huellas digitales en Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796694"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="de5c6-102">Usar la opción de desbloqueo de huellas digitales en Windows 10</span><span class="sxs-lookup"><span data-stu-id="de5c6-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="de5c6-103">**Habilitar Huella digital de Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="de5c6-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="de5c6-104">Para desbloquear Windows 10 con tu huella digital, debes configurar Windows Hello Fingerprint agregando (dejando que Windows aprenda a reconocer) al menos un dedo.</span><span class="sxs-lookup"><span data-stu-id="de5c6-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="de5c6-105">Ve a **Configuración > cuentas > opciones de inicio** de sesión (o haz clic [aquí).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="de5c6-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="de5c6-106">Aparecerán las opciones de inicio de sesión disponibles.</span><span class="sxs-lookup"><span data-stu-id="de5c6-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="de5c6-107">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="de5c6-107">For example:</span></span>

    ![Opciones de inicio de sesión.](media/sign-in-options.png)

2. <span data-ttu-id="de5c6-109">Haz clic o pulsa **en Huella digital de Windows Hello** y, a continuación, haz clic en **Configurar**.</span><span class="sxs-lookup"><span data-stu-id="de5c6-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="de5c6-110">En la ventana de instalación de Windows Hello, haga clic **en Introducción.**</span><span class="sxs-lookup"><span data-stu-id="de5c6-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="de5c6-111">El sensor de huella digital se activará y se te pedirá que coloques el dedo en el sensor:</span><span class="sxs-lookup"><span data-stu-id="de5c6-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sensor de huella digital.](media/fingerprint-sensor.png)

3. <span data-ttu-id="de5c6-113">Siga las instrucciones, que le pedirán que analice repetidamente el dedo.</span><span class="sxs-lookup"><span data-stu-id="de5c6-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="de5c6-114">Cuando esto termine, tendrás la opción de agregar otros dedos que quieras usar para el inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="de5c6-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="de5c6-115">La próxima vez que inicies sesión en Windows 10, tienes la opción de usar la huella digital para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="de5c6-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="de5c6-116">**Huella digital de Windows Hello no está disponible como opción de inicio de sesión**</span><span class="sxs-lookup"><span data-stu-id="de5c6-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="de5c6-117">Si la huella digital de Windows Hello no se muestra como una opción en las opciones de inicio de **sesión,** significa que Windows no conoce ningún lector de huellas digitales o escáner conectado al equipo, o que una directiva del sistema impide su uso (si, por ejemplo, el equipo está administrado por su lugar de trabajo).</span><span class="sxs-lookup"><span data-stu-id="de5c6-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="de5c6-118">Para solucionar problemas:</span><span class="sxs-lookup"><span data-stu-id="de5c6-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="de5c6-119">Selecciona el **botón Inicio** en la barra de tareas y busca Administrador **de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="de5c6-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="de5c6-120">Haga clic o pulse para abrir **el Administrador de dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="de5c6-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="de5c6-121">En el Administrador de dispositivos, expanda Dispositivos biométricos haciendo clic en su galón.</span><span class="sxs-lookup"><span data-stu-id="de5c6-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. <span data-ttu-id="de5c6-123">El escáner de huellas digitales debe aparecer como un dispositivo biométrico, como el escáner WBDI de Synaptics:</span><span class="sxs-lookup"><span data-stu-id="de5c6-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="de5c6-125">Si no se muestra el escáner de huellas digitales y el escáner está integrado en el equipo, vaya al sitio web del fabricante del equipo.</span><span class="sxs-lookup"><span data-stu-id="de5c6-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="de5c6-126">En la sección soporte técnico del modelo de pc, busca un controlador de Windows 10 para un escáner que puedas instalar.</span><span class="sxs-lookup"><span data-stu-id="de5c6-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="de5c6-127">Si el escáner es independiente del equipo (conectado a través de USB), vaya al sitio web del fabricante del escáner para buscar e instalar el software del controlador de dispositivo de Windows 10 para el modelo de escáner que tiene.</span><span class="sxs-lookup"><span data-stu-id="de5c6-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
