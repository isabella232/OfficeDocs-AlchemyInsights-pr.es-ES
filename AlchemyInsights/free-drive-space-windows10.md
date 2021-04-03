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
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="81fa4-102">Liberar espacio en disco en Windows 10</span><span class="sxs-lookup"><span data-stu-id="81fa4-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="81fa4-103">Estas son las dos opciones para liberar espacio en disco en Windows:</span><span class="sxs-lookup"><span data-stu-id="81fa4-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="81fa4-104">Liberar espacio en disco en Windows 10.</span><span class="sxs-lookup"><span data-stu-id="81fa4-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="81fa4-105">Liberar espacio para las actualizaciones de Windows 10 con dispositivo de almacenamiento externo.</span><span class="sxs-lookup"><span data-stu-id="81fa4-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="81fa4-106">Si todavía tiene poco espacio en disco después de usar el Liberador de espacio en disco, es posible que la carpeta Temp se esté llenando rápidamente con archivos de aplicación (.appx) usados por Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="81fa4-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="81fa4-107">Para solucionar este problema, restablezca la Store, borre la caché de Store y ejecute el solucionador de problemas de Windows Update.</span><span class="sxs-lookup"><span data-stu-id="81fa4-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="81fa4-108">Asegúrese de que Microsoft Store está cerrado antes de continuar con estos pasos.</span><span class="sxs-lookup"><span data-stu-id="81fa4-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="81fa4-109">**Paso 1: Restablecer Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="81fa4-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="81fa4-110">**Nota** Esta acción elimina de forma permanente los datos de la aplicación en el dispositivo, incluidos sus preferencias y detalles de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="81fa4-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="81fa4-111">Seleccione **Inicio** > **Configuración** > **Aplicaciones** > **Aplicaciones y características**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="81fa4-112">En la lista de aplicaciones, busque y seleccione Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="81fa4-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="81fa4-113">Seleccione **Opciones avanzadas**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="81fa4-114">Desplácese hacia abajo y seleccione **Restablecer** y, después, **Confirmar restablecimiento**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="81fa4-115">**Paso 2: Borrar la caché de Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="81fa4-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="81fa4-116">Pulse la tecla del logotipo de Windows + R para abrir el cuadro de diálogo Ejecutar.</span><span class="sxs-lookup"><span data-stu-id="81fa4-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="81fa4-117">Escriba wsreset.exe y seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="81fa4-118">Se abrirá una ventana del símbolo del sistema en blanco.</span><span class="sxs-lookup"><span data-stu-id="81fa4-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="81fa4-119">Después de unos 10 segundos, se cerrará la ventana y la Store se abrirá automáticamente.</span><span class="sxs-lookup"><span data-stu-id="81fa4-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="81fa4-120">**Paso 3: Restablecer Windows Update**</span><span class="sxs-lookup"><span data-stu-id="81fa4-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="81fa4-121">Seleccione **Inicio** > **Configuración** > **Actualización y seguridad** > **Solución de problemas**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="81fa4-122">Desplácese hacia abajo y seleccione **Windows Update** de la lista y, después, **Ejecute el solucionador de problemas**.</span><span class="sxs-lookup"><span data-stu-id="81fa4-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="81fa4-123">Reinicie el equipo y compruebe si todavía está experimentando el problema.</span><span class="sxs-lookup"><span data-stu-id="81fa4-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

