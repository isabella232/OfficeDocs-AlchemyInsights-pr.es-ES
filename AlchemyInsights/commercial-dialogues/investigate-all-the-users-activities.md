---
title: Investigar todas las actividades de los usuarios
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332360"
---
# <a name="investigate-all-the-users-activities"></a>Investigar todas las actividades de los usuarios

Este es el modo de hacerlo:

1. Realice una de las siguientes acciones:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

    **Nota:** Si ve un aviso de que necesita activar la característica, adelante y encándala ahora. Si la característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.

2. En la **pestaña Búsqueda** de la **página Auditoría,** configure las siguientes opciones:
   - **Intervalo de fecha y hora:** seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - **Actividades:** si está interesado en una actividad específica, selecciónelo en la lista; de lo contrario, el valor predeterminado **Mostrar resultados para todas las actividades** devuelve todas las actividades.
   - **Usuarios:** acepte el valor predeterminado en blanco para devolver resultados para todos los usuarios o escriba uno o varios usuarios.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.** Verá la dirección **IP,** **el usuario** y el nombre de **la** actividad.

4. Para descargar los resultados, **seleccione Exportar Descargar** todos los \> **resultados**.

5. Seleccione una actividad en los resultados para abrir el menú desplegable de detalles.

Para obtener más información, vea [Buscar en el registro de auditoría para investigar problemas de soporte técnico comunes.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
