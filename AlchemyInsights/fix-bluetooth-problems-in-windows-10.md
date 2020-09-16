---
title: Solucionar problemas de Bluetooth en Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730176"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="a95ff-102">Solucionar problemas de Bluetooth en Windows 10</span><span class="sxs-lookup"><span data-stu-id="a95ff-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="a95ff-103">Si falta el icono de Bluetooth o si no se puede activar o desactivar el Bluetooth, es posible que quiera ejecutar el solucionador de problemas de Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="a95ff-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="a95ff-104">[Abra la configuración de solución de problemas](ms-settings:troubleshoot), haga clic en **Bluetooth** , en **Buscar y solucionar otros problemas**, haga clic en **ejecutar el solucionador de problemas**.</span><span class="sxs-lookup"><span data-stu-id="a95ff-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="a95ff-105">Si no ve el icono de Bluetooth, pero Bluetooth aparece en el administrador de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="a95ff-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="a95ff-106">En el administrador de dispositivos, haga clic en **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="a95ff-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="a95ff-107">Mantén presionado (o haz clic con el botón derecho) en el nombre del adaptador Bluetooth y haz clic en **desinstalar dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="a95ff-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="a95ff-108">Apaga el dispositivo Windows, espera unos segundos y, a continuación, vuelve a encenderlo.</span><span class="sxs-lookup"><span data-stu-id="a95ff-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="a95ff-109">Windows intentará reinstalar el controlador.</span><span class="sxs-lookup"><span data-stu-id="a95ff-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="a95ff-110">Si has instalado recientemente actualizaciones de Windows 10 o actualizado a Windows 10, es posible que quieras comprobar las actualizaciones de los controladores:</span><span class="sxs-lookup"><span data-stu-id="a95ff-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="a95ff-111">En el administrador de dispositivos, haga clic en **Bluetooth**y, a continuación, haga clic en el nombre del adaptador Bluetooth (que puede incluir la palabra "radio").</span><span class="sxs-lookup"><span data-stu-id="a95ff-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="a95ff-112">Mantén presionado (o haz clic con el botón derecho) en el adaptador Bluetooth y, a continuación, haz clic en **Actualizar**  >  **búsqueda de controlador automáticamente para el software de controlador actualizado**.</span><span class="sxs-lookup"><span data-stu-id="a95ff-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="a95ff-113">Siga los pasos y, a continuación, haga clic en **cerrar**.</span><span class="sxs-lookup"><span data-stu-id="a95ff-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="a95ff-114">Si Windows no encuentra un nuevo controlador Bluetooth, visita el sitio web del fabricante del equipo y descarga el controlador Bluetooth más reciente desde allí.</span><span class="sxs-lookup"><span data-stu-id="a95ff-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="a95ff-115">Una vez descargado, haga clic en **Actualizar controlador**buscar en el  >  **equipo para el software de controlador**  >  **Busque** la ubicación en la que se almacenan los archivos del controlador > **Aceptar**  >  **Next**y siga los pasos para instalar.</span><span class="sxs-lookup"><span data-stu-id="a95ff-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="a95ff-116">Después de instalar el controlador actualizado, reinicie el equipo y, a continuación, compruebe si se ha corregido el problema de conexión.</span><span class="sxs-lookup"><span data-stu-id="a95ff-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="a95ff-117">Para obtener más información sobre cómo solucionar problemas de Bluetooth, vea el artículo completo, [solucionar problemas de Bluetooth en Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="a95ff-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
