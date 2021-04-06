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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Herramienta de diagnóstico del servicio para Windows Virtual Desktop

Windows Virtual Desktop (WVD) ofrece una herramienta de diagnóstico que permite a los administradores identificar errores en una sola interfaz. Esta herramienta registra información relacionada con el diagnóstico, siempre que la use alguien con un rol de WVD asignado. Cada registro contiene información sobre el rol de WVD implicado en la actividad, los mensajes de error que aparecen durante la sesión e información sobre el espacio empresarial y el usuario. Azure Log Analytics se puede configurar para capturar el registro de actividades creado por la herramienta de diagnóstico. Para ello, siga estos pasos:

1. Cree un área de trabajo de Log Analytics con [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Conecte los equipos con Windows a Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenga el id. de área de trabajo y la clave principal de su área de trabajo. El asistente para la configuración necesita esta información para configurar correctamente el agente y asegurarse de que se pueda comunicar con Azure Monitor.

1. [Inserte datos de diagnóstico en el área de trabajo](https://go.microsoft.com/fwlink/?linkid=2128284). Puede insertar datos de diagnóstico desde su espacio empresarial de WVD en Log Analytics para su área de trabajo.

1. [Identifique y diagnostique](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas internos o externos en relación con WVD.

Para obtener más información sobre cómo configurar la herramienta de diagnóstico del servicio para WVD, vea Usar Log Analytics para la característica de diagnóstico.