---
title: Se ha resuelto el problema con el administrador de trabajos de impresión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083982"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="454be-102">Se ha resuelto el problema con el administrador de trabajos de impresión</span><span class="sxs-lookup"><span data-stu-id="454be-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="454be-103">Si su dispositivo se ha actualizado con la **compilación de sistema operativo 19041.329** de Windows 10, es posible que haya observado un fallo de impresión en ciertas impresoras.</span><span class="sxs-lookup"><span data-stu-id="454be-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="454be-104">Puede que el administrador de trabajos de impresión indique un error o que se cierre de manera inesperada al intentar imprimir y que la impresora afectada no produzca ningún resultado.</span><span class="sxs-lookup"><span data-stu-id="454be-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="454be-105">Este problema se resuelve en la compilación de sistema operativo **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="454be-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="454be-106">**Investigación en curso**</span><span class="sxs-lookup"><span data-stu-id="454be-106">**Ongoing investigation**</span></span>

<span data-ttu-id="454be-107">Es posible que el archivo del Servicio de subsistema de autoridad de seguridad local, o LSASS (**Isass.exe**), produzca errores en algunos dispositivos y genere el siguiente mensaje de error: "Un proceso crítico del sistema, C:\WINDOWS\system32\Isass.exe, ha producido un error con el código de estado c0000008.</span><span class="sxs-lookup"><span data-stu-id="454be-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="454be-108">Es necesario reiniciar el equipo ahora".</span><span class="sxs-lookup"><span data-stu-id="454be-108">The machine must now be restarted".</span></span>  <span data-ttu-id="454be-109">**Microsoft está trabajando en una solución y le ofrecerá una actualización en una versión futura.**</span><span class="sxs-lookup"><span data-stu-id="454be-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="454be-110">Para más información, consulte los [problemas conocidos de la versión 2004 de Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="454be-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>