---
title: 0x8004de40 error al iniciar OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813669"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="82da4-102">0x8004de40 error al iniciar OneDrive</span><span class="sxs-lookup"><span data-stu-id="82da4-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="82da4-103">Si recibe un **error** 0x8004de40 al iniciar sesión en OneDrive, reinicie el equipo mientras está conectado al dominio de trabajo o escuela.</span><span class="sxs-lookup"><span data-stu-id="82da4-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="82da4-104">Si recibe este error después de reiniciar, pruébalo mientras está conectado al dominio de trabajo o escuela:</span><span class="sxs-lookup"><span data-stu-id="82da4-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="82da4-105">Haga clic en Inicio y escriba **cmd** **o** símbolo del sistema en el cuadro de búsqueda, haga clic con el botón secundario en la aplicación del símbolo del sistema y seleccione Ejecutar como **administrador.**</span><span class="sxs-lookup"><span data-stu-id="82da4-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="82da4-106">Si se le pide una contraseña de administrador o una confirmación, escriba la contraseña o haga clic en **Permitir**.</span><span class="sxs-lookup"><span data-stu-id="82da4-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="82da4-107">En la ventana Símbolo del sistema, escriba **dsregcmd /leave**  y espere a que se complete el comando.</span><span class="sxs-lookup"><span data-stu-id="82da4-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="82da4-108">A **continuación, escriba dsregcmd /join** y espere a que se complete el comando.</span><span class="sxs-lookup"><span data-stu-id="82da4-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="82da4-109">Reinicie el equipo.</span><span class="sxs-lookup"><span data-stu-id="82da4-109">Reboot your computer.</span></span>
