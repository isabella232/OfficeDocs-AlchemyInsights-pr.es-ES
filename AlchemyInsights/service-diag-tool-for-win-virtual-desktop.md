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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Herramienta de diagnóstico de servicios para el escritorio virtual de Windows

El escritorio virtual de Windows (WVD) ofrece una herramienta de diagnóstico que permite a los administradores identificar los errores a través de una única interfaz. Esta herramienta registra información relacionada con los diagnósticos cada vez que un usuario al que se le asigna un rol de WVD usa WVD. Cada registro contiene información sobre el rol WVD implicado en la actividad, los mensajes de error que aparecen durante la sesión y la información sobre el inquilino y el usuario. El análisis de registros de Azure se puede configurar para capturar el registro de actividades creado por la herramienta de diagnóstico. A continuación se describe cómo:

1. Cree un área de trabajo de análisis de registros con [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Conecte los equipos Windows a Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenga el identificador del área de trabajo y la clave principal del área de trabajo. El Asistente para la instalación necesita esta información para configurar correctamente el agente y para asegurarse de que se puede comunicar con Azure monitor.
1. [Insertar datos de diagnóstico en el área de trabajo](https://go.microsoft.com/fwlink/?linkid=2128284). Puede insertar datos de diagnóstico de su inquilino de WVD en el análisis de registros del área de trabajo.
1. [Identificar y diagnosticar problemas](https://go.microsoft.com/fwlink/?linkid=2128338) internos o externos en relación con WVD.

Para obtener más información acerca de la configuración de la herramienta de diagnóstico de servicios para WVD, consulte [use análisis de registros para la característica diagnósticos](https://go.microsoft.com/fwlink/?linkid=2128084).
