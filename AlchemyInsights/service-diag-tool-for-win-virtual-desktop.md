---
title: Herramienta de diagnóstico de servicios para el escritorio virtual de Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665840"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b7807-102">Herramienta de diagnóstico de servicios para el escritorio virtual de Windows</span><span class="sxs-lookup"><span data-stu-id="b7807-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b7807-103">El escritorio virtual de Windows (WVD) ofrece una herramienta de diagnóstico que permite a los administradores identificar los errores a través de una única interfaz.</span><span class="sxs-lookup"><span data-stu-id="b7807-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b7807-104">Esta herramienta registra información relacionada con los diagnósticos cada vez que un usuario al que se le asigna un rol de WVD usa WVD.</span><span class="sxs-lookup"><span data-stu-id="b7807-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b7807-105">Cada registro contiene información sobre el rol WVD implicado en la actividad, los mensajes de error que aparecen durante la sesión y la información sobre el inquilino y el usuario.</span><span class="sxs-lookup"><span data-stu-id="b7807-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b7807-106">El análisis de registros de Azure se puede configurar para capturar el registro de actividades creado por la herramienta de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="b7807-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="b7807-107">A continuación se describe cómo:</span><span class="sxs-lookup"><span data-stu-id="b7807-107">Here's how:</span></span>

1. <span data-ttu-id="b7807-108">Cree un área de trabajo de análisis de registros con [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="b7807-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="b7807-109">[Conecte los equipos Windows a Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="b7807-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b7807-110">Obtenga el identificador del área de trabajo y la clave principal del área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="b7807-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b7807-111">El Asistente para la instalación necesita esta información para configurar correctamente el agente y para asegurarse de que se puede comunicar con Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="b7807-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="b7807-112">[Insertar datos de diagnóstico en el área de trabajo](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="b7807-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b7807-113">Puede insertar datos de diagnóstico de su inquilino de WVD en el análisis de registros del área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="b7807-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="b7807-114">[Identificar y diagnosticar problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos o externos en relación con WVD.</span><span class="sxs-lookup"><span data-stu-id="b7807-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b7807-115">Para obtener más información acerca de la configuración de la herramienta de diagnóstico de servicios para WVD, consulte [use análisis de registros para la característica diagnósticos](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="b7807-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
