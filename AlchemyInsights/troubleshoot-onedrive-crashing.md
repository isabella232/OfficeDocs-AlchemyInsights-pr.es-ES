---
title: Solución de problemas de bloqueo de OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826216"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6e972-102">Solución de problemas de bloqueo de OneDrive</span><span class="sxs-lookup"><span data-stu-id="6e972-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6e972-103">Si OneDrive se bloquea de forma repetida, pruebe estos pasos de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="6e972-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6e972-104">**Asegúrese de que las claves del registro no estén configuradas:**</span><span class="sxs-lookup"><span data-stu-id="6e972-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6e972-105">Abra el Editor del Registro y vaya a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6e972-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6e972-106">Si existe la clave DisableFileSyncNGSC y esta está establecida en 1, abra la clave y cambie el valor a 0.</span><span class="sxs-lookup"><span data-stu-id="6e972-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6e972-107">Vaya a Inicio para iniciar OneDrive manualmente.</span><span class="sxs-lookup"><span data-stu-id="6e972-107">Manually launch OneDrive by going to Start</span></span> ![Presione la tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6e972-109">, escriba OneDrive en el cuadro de búsqueda y luego haga clic en la aplicación de escritorio de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6e972-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6e972-110">**Restablezca OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6e972-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6e972-111">Notas:</span><span class="sxs-lookup"><span data-stu-id="6e972-111">Notes:</span></span>

- <span data-ttu-id="6e972-112">Al restablecer OneDrive, todas las conexiones de sincronización existentes se desconectarán (incluida la de OneDrive personal, si está configurada).</span><span class="sxs-lookup"><span data-stu-id="6e972-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6e972-113">Si restablece OneDrive en su equipo, no perderá sus archivos ni su información.</span><span class="sxs-lookup"><span data-stu-id="6e972-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6e972-114">**Para restablecer OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6e972-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6e972-115">Presione las teclas Windows y R para abrir el cuadro de diálogo Ejecutar.</span><span class="sxs-lookup"><span data-stu-id="6e972-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6e972-116">Escriba %localappdata%\Microsoft\OneDrive\onedrive.exe/reset y presione Aceptar.</span><span class="sxs-lookup"><span data-stu-id="6e972-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6e972-117">Es posible que aparezca momentáneamente una ventana de comandos.</span><span class="sxs-lookup"><span data-stu-id="6e972-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6e972-118">Vaya a Inicio para iniciar OneDrive manualmente.</span><span class="sxs-lookup"><span data-stu-id="6e972-118">Manually launch OneDrive by going to Start</span></span> ![Presione la tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6e972-120">, escriba OneDrive en el cuadro de búsqueda y luego haga clic en la aplicación de escritorio de OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6e972-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6e972-121">Notas:</span><span class="sxs-lookup"><span data-stu-id="6e972-121">Notes:</span></span>

- <span data-ttu-id="6e972-122">Si antes del restablecimiento elige sincronizar solo algunas carpetas, deberá hacerlo de nuevo una vez que se haya completado la sincronización.</span><span class="sxs-lookup"><span data-stu-id="6e972-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6e972-123">Lea  [Elegir qué carpetas de OneDrive se sincronizarán con su equipo](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="6e972-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6e972-124">Tendrá que seguir estos pasos con su OneDrive personal y con OneDrive para la Empresa.</span><span class="sxs-lookup"><span data-stu-id="6e972-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>