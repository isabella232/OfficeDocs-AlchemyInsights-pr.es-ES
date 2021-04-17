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
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828169"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="78683-102">Configuración de inicio en Windows 10</span><span class="sxs-lookup"><span data-stu-id="78683-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="78683-103">**Cambiar las aplicaciones que se ejecutan automáticamente al inicio**</span><span class="sxs-lookup"><span data-stu-id="78683-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="78683-104">Ve a [Configuración > aplicaciones > inicio.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="78683-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="78683-105">Asegúrate de que cualquier aplicación que quieras ejecutar en el inicio esté **activada**.</span><span class="sxs-lookup"><span data-stu-id="78683-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="78683-106">**Agregar una aplicación para que se ejecute automáticamente al inicio**</span><span class="sxs-lookup"><span data-stu-id="78683-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="78683-107">Haz clic o pulsa **en Inicio** y busca la aplicación que quieres ejecutar al inicio.</span><span class="sxs-lookup"><span data-stu-id="78683-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="78683-108">Haga clic con el botón secundario en la aplicación, haga clic en **Más** y, a continuación, haga clic **en Abrir ubicación del archivo**.</span><span class="sxs-lookup"><span data-stu-id="78683-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="78683-109">Se abre la ubicación donde se guarda el acceso directo a la aplicación.</span><span class="sxs-lookup"><span data-stu-id="78683-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="78683-110">Si no hay ninguna opción para la ubicación de abrir archivo, significa que la aplicación no se puede ejecutar al inicio.</span><span class="sxs-lookup"><span data-stu-id="78683-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="78683-111">Con la ubicación del archivo abierta, presione la tecla **del logotipo de Windows + R**, escriba **shell:startup** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="78683-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="78683-112">Se abre la carpeta Inicio.</span><span class="sxs-lookup"><span data-stu-id="78683-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="78683-113">Copie y pegue el acceso directo a la aplicación desde la ubicación del archivo a la carpeta Inicio.</span><span class="sxs-lookup"><span data-stu-id="78683-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="78683-114">**Opciones avanzadas de inicio (incluido el modo seguro, la configuración de UEFI y el arranque desde otro dispositivo)**</span><span class="sxs-lookup"><span data-stu-id="78683-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="78683-115">Guarde el trabajo y cierre los documentos abiertos, ya que estos pasos reiniciarán el equipo.</span><span class="sxs-lookup"><span data-stu-id="78683-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="78683-116">Vaya a [Configuración > Actualizar & seguridad > recuperación](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="78683-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="78683-117">En **Inicio avanzado,** haga clic **en Reiniciar ahora**.</span><span class="sxs-lookup"><span data-stu-id="78683-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="78683-118">Después de reiniciar el equipo en la pantalla elegir una opción:</span><span class="sxs-lookup"><span data-stu-id="78683-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="78683-119">Para arrancar desde un dispositivo como una unidad USB, haga clic **en Usar un dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="78683-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="78683-120">Para especificar la configuración de UEFI (a veces denominada configuración del BIOS), haga clic en Solucionar problemas > opciones avanzadas > configuración de **firmware uefi**.</span><span class="sxs-lookup"><span data-stu-id="78683-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="78683-121">Para entrar en modo seguro o cambiar la configuración de inicio avanzada, haga clic en Solucionar problemas **> opciones** avanzadas > configuración de inicio y, a continuación, haga clic en **Reiniciar**.</span><span class="sxs-lookup"><span data-stu-id="78683-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="78683-122">Es posible que se te pida que escribas la [clave de recuperación de BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="78683-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="78683-123">Después de reiniciar de nuevo el equipo, haz clic en la configuración de inicio que quieras usar.</span><span class="sxs-lookup"><span data-stu-id="78683-123">After your PC restarts again, click the startup setting you want to use.</span></span>