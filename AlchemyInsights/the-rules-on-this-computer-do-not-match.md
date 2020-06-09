---
title: 'Error: las reglas de este equipo no coinciden'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618030"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Error: las reglas de este equipo no coinciden

Para ver el estado actualizado de este problema conocido, consulte las [reglas de este equipo no coinciden con las reglas de Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

El equipo de Outlook ha implementado una corrección en la compilación 12928,10000. La corrección ya está en una hora de Insider rápida y se dirigirá a la canal mensual en el 2020 de junio de junio. Una vez que tenga la compilación fija, puede que reciba el mensaje "¿qué reglas desea mantener" una última vez. Elija servidor cuando se le solicite y, a continuación, vuelva a Outlook y vuelva a habilitar las reglas que se hayan deshabilitado.

Hasta que la corrección esté disponible, use la siguiente solución alternativa:

**Solución**: en informes recientes, el problema se debe a aquellos que solo han creado reglas de cliente en el escritorio de Outlook. Si sigue teniendo el problema, considere la posibilidad de eliminar las reglas y, a continuación, cree y modifique las reglas solo en OWA (Outlook Web App) hasta que se resuelva el problema.

Si no puede eliminar las reglas manualmente, puede ejecutar un comando de Outlook al iniciar Outlook ejecutando Outlook. exe/cleanrules. Se eliminarán las reglas de cliente y de servidor. Se eliminarán todas las reglas de todas las cuentas del perfil de Outlook. Este comando se documenta en el artículo modificadores de la línea de comandos.