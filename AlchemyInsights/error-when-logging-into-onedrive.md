---
title: error de 0x8004de40 al iniciar OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816024"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="da16a-102">error de 0x8004de40 al iniciar OneDrive</span><span class="sxs-lookup"><span data-stu-id="da16a-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="da16a-103">Si recibe un error **0x8004de40** al iniciar sesión en OneDrive, reinicie el equipo mientras está conectado a su dominio profesional o educativo.</span><span class="sxs-lookup"><span data-stu-id="da16a-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="da16a-104">Si recibe este error después de reiniciar, pruébelo mientras está conectado a su dominio profesional o educativo:</span><span class="sxs-lookup"><span data-stu-id="da16a-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="da16a-105">Haga clic en Inicio y escriba **cmd** o **símbolo del sistema**  en el cuadro de búsqueda, haga clic con el botón secundario en la aplicación de símbolo del sistema y seleccione  **Ejecutar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="da16a-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="da16a-106">Si se le pide una contraseña de administrador o una confirmación, escriba la contraseña o haga clic en **permitir** .</span><span class="sxs-lookup"><span data-stu-id="da16a-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="da16a-107">En la ventana del símbolo del sistema, escriba **dsregcmd/Leave**  y espere a que se complete el comando.</span><span class="sxs-lookup"><span data-stu-id="da16a-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="da16a-108">A continuación, escriba **dsregcmd/join** y espere a que se complete el comando.</span><span class="sxs-lookup"><span data-stu-id="da16a-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="da16a-109">Reinicie el equipo.</span><span class="sxs-lookup"><span data-stu-id="da16a-109">Reboot your computer.</span></span>
