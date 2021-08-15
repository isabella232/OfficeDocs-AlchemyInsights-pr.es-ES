---
title: 'Error: las reglas de este equipo no coinciden'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981130"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Error: las reglas de este equipo no coinciden

Para ver el estado actualizado de este problema conocido, vea [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

El Outlook ha implementado una corrección en la compilación 12928.10000. The fix is already at Insider Fast and will go to Monthly Channel in late June 2020. Una vez que tenga la compilación fija, puede obtener el mensaje "Qué reglas desea conservar" una última vez. Elija Servidor cuando se le pida y, a continuación, vuelva a Outlook y vuelva a habilitar las reglas que se han deshabilitado.

Hasta que la corrección esté disponible, use la siguiente solución alternativa:

**Solución** alternativa: En informes recientes, el problema se ha producido para aquellos que solo han creado reglas de cliente en Outlook escritorio. Si continúa con el problema, considere la posibilidad de eliminar las reglas y, a continuación, crear y editar reglas solo en OWA (Outlook Web App) hasta que se resuelva el problema.

Si no puede eliminar las reglas manualmente, puede ejecutar un comando Outlook al iniciar Outlook ejecutando Outlook.exe /cleanrules. Esto eliminará las reglas de cliente y de servidor. Eliminará todas las reglas de todas las cuentas del Outlook perfil. Este comando se documenta más adelante en el artículo Modificadores de línea de comandos.

