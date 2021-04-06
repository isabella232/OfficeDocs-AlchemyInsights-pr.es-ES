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
# <a name="identify-windows-virtual-desktop-issues"></a>Identificar problemas de Windows Virtual Desktop

Diagnóstico de Windows Virtual Desktop usa solo un cmdlet de PowerShell, pero contiene muchos parámetros opcionales para ayudar a limitar y aislar los problemas. Para empezar: 

1. Descargar e importar el módulo de PowerShell Windows Virtual Desktop Para más información, consulte [Cmdlets de Windows Virtual Desktop para Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Ejecute el siguiente cmdlet para iniciar sesión en su cuenta:
    
    Ejemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOTA:** Todas las consultas que usan PowerShell deben incluir los parámetros -UserName o -ActivityID. Para obtener más información sobre las capacidades de supervisión, consulte [Log Analytics para la característica de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).

Para filtrar actividades de diagnóstico por usuario, ejecute el cmdlet siguiente:

Ejemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Hay una lista de filtros que puede ejecutar para diagnosticar problemas. Para obtener más información sobre cómo diagnosticar problemas, consulte [Identificar y diagnosticar problemas de Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Para obtener más información sobre los errores comunes, consulte [Escenarios de errores comunes](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
