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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898395"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="35cb2-102">Liberar espacio en disco en Windows 10</span><span class="sxs-lookup"><span data-stu-id="35cb2-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="35cb2-103">Estas son las dos opciones para liberar espacio en disco en Windows:</span><span class="sxs-lookup"><span data-stu-id="35cb2-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="35cb2-104">Liberar espacio en disco en Windows 10.</span><span class="sxs-lookup"><span data-stu-id="35cb2-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="35cb2-105">Liberar espacio para las actualizaciones de Windows 10 con dispositivo de almacenamiento externo.</span><span class="sxs-lookup"><span data-stu-id="35cb2-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="35cb2-106">Si todavía tiene poco espacio en disco después de usar el Liberador de espacio en disco, es posible que la carpeta Temp se esté llenando rápidamente con archivos de aplicación (.appx) usados por Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="35cb2-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="35cb2-107">Para solucionar este problema, restablezca la Store, borre la caché de Store y ejecute el solucionador de problemas de Windows Update.</span><span class="sxs-lookup"><span data-stu-id="35cb2-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="35cb2-108">Asegúrese de que Microsoft Store está cerrado antes de continuar con estos pasos.</span><span class="sxs-lookup"><span data-stu-id="35cb2-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="35cb2-109">**Paso 1: Restablecer Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="35cb2-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="35cb2-110">**Nota** Esta acción elimina de forma permanente los datos de la aplicación en el dispositivo, incluidos sus preferencias y detalles de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="35cb2-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="35cb2-111">Seleccione **Inicio** > **Configuración** > **Aplicaciones** > **Aplicaciones y características**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="35cb2-112">En la lista de aplicaciones, busque y seleccione Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="35cb2-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="35cb2-113">Seleccione **Opciones avanzadas**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="35cb2-114">Desplácese hacia abajo y seleccione **Restablecer** y, después, **Confirmar restablecimiento**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="35cb2-115">**Paso 2: Borrar la caché de Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="35cb2-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="35cb2-116">Pulse la tecla del logotipo de Windows + R para abrir el cuadro de diálogo Ejecutar.</span><span class="sxs-lookup"><span data-stu-id="35cb2-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="35cb2-117">Escriba wsreset.exe y seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="35cb2-118">Se abrirá una ventana del símbolo del sistema en blanco.</span><span class="sxs-lookup"><span data-stu-id="35cb2-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="35cb2-119">Después de unos 10 segundos, se cerrará la ventana y la Store se abrirá automáticamente.</span><span class="sxs-lookup"><span data-stu-id="35cb2-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="35cb2-120">**Paso 3: Restablecer Windows Update**</span><span class="sxs-lookup"><span data-stu-id="35cb2-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="35cb2-121">Seleccione **Inicio** > **Configuración** > **Actualización y seguridad** > **Solución de problemas**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="35cb2-122">Desplácese hacia abajo y seleccione **Windows Update** de la lista y, después, **Ejecute el solucionador de problemas**.</span><span class="sxs-lookup"><span data-stu-id="35cb2-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="35cb2-123">Reinicie el equipo y compruebe si todavía está experimentando el problema.</span><span class="sxs-lookup"><span data-stu-id="35cb2-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

