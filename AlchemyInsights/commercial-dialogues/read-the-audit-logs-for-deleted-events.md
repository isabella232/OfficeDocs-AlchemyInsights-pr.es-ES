---
title: Leer los registros de auditoría para eventos eliminados
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324750"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leer los registros de auditoría para eventos eliminados

Este es el modo de hacerlo:

1. Realice una de las siguientes acciones:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

    **Nota:** Si ve un aviso de que necesita activar la característica, adelante y encándala ahora. Si la característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.

2. En la **pestaña Búsqueda** de la **página Auditoría,** configure las siguientes opciones:
   - **Intervalo de fecha y hora:** seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - **Actividades:** escriba **Exchange de buzón de correo** y, a continuación, seleccione los siguientes valores:
     - **Mensajes eliminados de la carpeta elementos eliminados**
     - **Mensajes movidos a la carpeta Elementos eliminados**

       Cuando haya terminado, haga clic fuera del panel para minimizar el **panel** Actividades.

   - **Usuarios:** acepte el valor predeterminado en blanco para devolver resultados para todos los usuarios o escriba uno o varios usuarios.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. Seleccione una actividad en los resultados para abrir el menú desplegable de detalles. Se muestra información adicional sobre el elemento eliminado, como la línea de asunto y la ubicación del elemento cuando se eliminó, en el **campo AffectedItems.**

   **Nota:** No puede restaurar elementos eliminados con la característica de registro de auditoría. Para restaurar elementos eliminados, vea [Recuperar mensajes de correo electrónico eliminados en Outlook en la Web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Para obtener más información, [vea Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
