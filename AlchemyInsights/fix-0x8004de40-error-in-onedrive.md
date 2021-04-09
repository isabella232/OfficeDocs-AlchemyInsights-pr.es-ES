---
title: Corregir 0x8004de40 error en OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649765"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ddda9-102">Corregir 0x8004de40 error en OneDrive</span><span class="sxs-lookup"><span data-stu-id="ddda9-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ddda9-103">Si estás ejecutando Windows 7 y recibes este error, actualiza para habilitar [TLS 1.1 y TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)como protocolos seguros predeterminados en WinHTTP en Windows .</span><span class="sxs-lookup"><span data-stu-id="ddda9-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="ddda9-104">Si estás ejecutando Windows 10 y recibes un 0x8004de40 error con OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ddda9-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ddda9-105">Reinicie el equipo afectado mientras está conectado al dominio de directorio de Acitve.</span><span class="sxs-lookup"><span data-stu-id="ddda9-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ddda9-106">Si un reinicio no soluciona el problema, desenlace y vuelva a unirse al dispositivo desde Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ddda9-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ddda9-107">**Nota:** Debe estar en la red corporativa mientras realiza estos pasos.</span><span class="sxs-lookup"><span data-stu-id="ddda9-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ddda9-108">No realice estos pasos cuando no esté conectado a la infraestructura corporativa (por ejemplo, mientras viaja).</span><span class="sxs-lookup"><span data-stu-id="ddda9-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="ddda9-109">Abra un símbolo del sistema con privilegios elevados **seleccionando Inicio**, haga clic con el botón secundario en Símbolo del sistema y, a continuación, **seleccione Ejecutar como administrador**. </span><span class="sxs-lookup"><span data-stu-id="ddda9-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="ddda9-110">Escriba *dsregcmd /leave y* presione **Entrar**.</span><span class="sxs-lookup"><span data-stu-id="ddda9-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="ddda9-111">Cuando haya finalizado, escriba *dsregcmd /join y* presione **Entrar**.</span><span class="sxs-lookup"><span data-stu-id="ddda9-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="ddda9-112">Cuando se complete, cierre el símbolo del sistema.</span><span class="sxs-lookup"><span data-stu-id="ddda9-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="ddda9-113">Reinicie el equipo e inicie sesión en OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ddda9-113">Reboot the computer, and log into OneDrive.</span></span>