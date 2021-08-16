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
ms.openlocfilehash: 398496448089d4480119a2eb21221dc11f13c6c1f3bcbd931d6c18033f2e734e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987586"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identificar problemas de Windows Virtual Desktop

Diagnóstico de Windows Virtual Desktop usa solo un cmdlet de PowerShell, pero contiene muchos parámetros opcionales para ayudar a limitar y aislar los problemas. 

1. Descargar e importar el módulo de PowerShell Windows Virtual Desktop Para más información, consulte [Cmdlets de Windows Virtual Desktop para Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Ejecute el siguiente cmdlet para iniciar sesión en su cuenta:
    
    Ejemplo: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOTA:** Todas las consultas que usan PowerShell deben incluir los parámetros -UserName o -ActivityID. Para obtener más información sobre las capacidades de supervisión, consulte [Log Analytics para la característica de diagnóstico](https://go.microsoft.com/fwlink/?linkid=2126847).

Para filtrar actividades de diagnóstico por usuario, ejecute el cmdlet siguiente:

Ejemplo: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Hay una lista de filtros que puede ejecutar para diagnosticar problemas. Para obtener más información sobre cómo diagnosticar problemas, consulte [Identificar y diagnosticar problemas de Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Para obtener más información sobre los errores comunes, consulte [Escenarios de errores comunes](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
