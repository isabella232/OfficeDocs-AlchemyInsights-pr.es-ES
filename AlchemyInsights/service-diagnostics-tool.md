---
title: Herramienta de diagnóstico del servicio para Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590322"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="0a966-102">Herramienta de diagnóstico del servicio para Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="0a966-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="0a966-103">Windows Virtual Desktop (WVD) ofrece una herramienta de diagnóstico que permite a los administradores identificar errores en una sola interfaz.</span><span class="sxs-lookup"><span data-stu-id="0a966-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="0a966-104">Esta herramienta registra información relacionada con el diagnóstico, siempre que la use alguien con un rol de WVD asignado.</span><span class="sxs-lookup"><span data-stu-id="0a966-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="0a966-105">Cada registro contiene información sobre el rol de WVD implicado en la actividad, los mensajes de error que aparecen durante la sesión e información sobre el espacio empresarial y el usuario.</span><span class="sxs-lookup"><span data-stu-id="0a966-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="0a966-106">Azure Log Analytics se puede configurar para capturar el registro de actividades creado por la herramienta de diagnóstico. Para ello, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="0a966-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="0a966-107">Cree un área de trabajo de Log Analytics con [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="0a966-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="0a966-108">[Conecte los equipos con Windows a Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="0a966-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="0a966-109">Obtenga el id. de área de trabajo y la clave principal de su área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0a966-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="0a966-110">El asistente para la configuración necesita esta información para configurar correctamente el agente y asegurarse de que se pueda comunicar con Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="0a966-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="0a966-111">[Inserte datos de diagnóstico en el área de trabajo](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="0a966-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="0a966-112">Puede insertar datos de diagnóstico desde su espacio empresarial de WVD en Log Analytics para su área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0a966-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="0a966-113">[Identifique y diagnostique](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas internos o externos en relación con WVD.</span><span class="sxs-lookup"><span data-stu-id="0a966-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="0a966-114">Para obtener más información sobre cómo configurar la herramienta de diagnóstico del servicio para WVD, vea Usar Log Analytics para la característica de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="0a966-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>