---
title: Herramienta de diagnóstico del servicio para Windows Virtual Desktop
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052403"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Herramienta de diagnóstico del servicio para Windows Virtual Desktop

Windows Virtual Desktop (WVD) ofrece una herramienta de diagnóstico que permite a los administradores identificar errores en una sola interfaz. Esta herramienta registra información relacionada con el diagnóstico, siempre que la use alguien con un rol de WVD asignado. Cada registro contiene información sobre el rol de WVD implicado en la actividad, los mensajes de error que aparecen durante la sesión e información sobre el espacio empresarial y el usuario. Azure Log Analytics se puede configurar para capturar el registro de actividad creado por la herramienta de diagnóstico. A continuación se muestra cómo hacerlo:

1. Cree un área de trabajo de Log Analytics con [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Conecte los equipos con Windows a Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenga el id. de área de trabajo y la clave principal de su área de trabajo. El asistente para la configuración necesita esta información para configurar correctamente el agente y asegurarse de que se pueda comunicar con Azure Monitor.
1. [Inserte datos de diagnóstico en el área de trabajo](https://go.microsoft.com/fwlink/?linkid=2128284). Puede insertar datos de diagnóstico desde su espacio empresarial de WVD en Log Analytics para su área de trabajo.
1. [Identificar y diagnosticar problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos o externos en relación con WVD.

Para obtener más información sobre cómo configurar la herramienta de diagnóstico de servicio para WVD, consulte [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).
