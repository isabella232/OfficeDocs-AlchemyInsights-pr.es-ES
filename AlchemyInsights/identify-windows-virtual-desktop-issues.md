---
title: Identificar problemas de Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590321"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="a1245-102">Identificar problemas de Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="a1245-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="a1245-103">Diagnóstico de Windows Virtual Desktop usa solo un cmdlet de PowerShell, pero contiene muchos parámetros opcionales para ayudar a limitar y aislar los problemas.</span><span class="sxs-lookup"><span data-stu-id="a1245-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="a1245-104">Para empezar:</span><span class="sxs-lookup"><span data-stu-id="a1245-104">To get started:</span></span> 

1. <span data-ttu-id="a1245-105">Descargar e importar el módulo de PowerShell Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="a1245-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="a1245-106">Para más información, consulte [Cmdlets de Windows Virtual Desktop para Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="a1245-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="a1245-107">Ejecute el siguiente cmdlet para iniciar sesión en su cuenta:</span><span class="sxs-lookup"><span data-stu-id="a1245-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="a1245-108">Ejemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="a1245-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="a1245-109">**NOTA:** Todas las consultas que usan PowerShell deben incluir los parámetros -UserName o -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="a1245-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="a1245-110">Para obtener más información sobre las capacidades de supervisión, consulte [Log Analytics para la característica de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="a1245-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="a1245-111">Para filtrar actividades de diagnóstico por usuario, ejecute el cmdlet siguiente:</span><span class="sxs-lookup"><span data-stu-id="a1245-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="a1245-112">Ejemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="a1245-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="a1245-113">Hay una lista de filtros que puede ejecutar para diagnosticar problemas.</span><span class="sxs-lookup"><span data-stu-id="a1245-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="a1245-114">Para obtener más información sobre cómo diagnosticar problemas, consulte [Identificar y diagnosticar problemas de Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="a1245-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="a1245-115">Para obtener más información sobre los errores comunes, consulte [Escenarios de errores comunes](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="a1245-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
