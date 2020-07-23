---
title: Solucionar problemas de sincronización de contraseñas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387894"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c8e5f-102">Solucionar problemas de sincronización de contraseñas</span><span class="sxs-lookup"><span data-stu-id="c8e5f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c8e5f-103">Para solucionar problemas de sincronización de contraseñas, empiece con esta tarea de solución de problemas de AAD Connect para determinar por qué las contraseñas no se sincronizan.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="c8e5f-104">Para empezar, vaya a [Manage Direct Sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="c8e5f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="c8e5f-105">Abra una nueva sesión de Windows PowerShell en su servidor de Azure AD Connect y seleccione la opción **Ejecutar como administrador** .</span><span class="sxs-lookup"><span data-stu-id="c8e5f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c8e5f-106">Ejecute Set-ExecutionPolicy RemoteSigned o Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="c8e5f-107">Inicie el Asistente de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c8e5f-108">Vaya a la página tareas adicionales > **solucionar problemas**a  >  **continuación**.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="c8e5f-109">Seleccione **iniciar** para abrir el menú solución de problemas de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="c8e5f-110">Seleccione **solucionar problemas de sincronización de contraseñas**.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="c8e5f-111">El problema suele ser que una contraseña no está sincronizada para una cuenta de usuario específica.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="c8e5f-112">**Notas** Se produce un error en la sincronización de contraseña si la última sincronización de contraseña correcta ha transcurrido algún tiempo.</span><span class="sxs-lookup"><span data-stu-id="c8e5f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="c8e5f-113">Para obtener más información sobre cómo solucionar problemas de sincronización de contraseñas, vea [solucionar problemas de sincronización de hash de contraseña con Azure ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c8e5f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>