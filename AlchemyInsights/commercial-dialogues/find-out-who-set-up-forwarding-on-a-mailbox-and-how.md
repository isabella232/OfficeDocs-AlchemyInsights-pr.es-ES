---
title: Descubra quién configura el reenvío en un buzón y cómo
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317825"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quién configura el reenvío en un buzón y cómo

Si el reenvío externo se estableció en un buzón, la actividad se auditará como parte del cmdlet **Set-Mailbox.** Este es el modo de encontrar la actividad en el registro de auditoría:

1. Realice una de las siguientes acciones:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

   **Nota:** Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.

2. En la **página Auditoría,** compruebe que la **pestaña** Búsqueda está seleccionada y, a continuación, configure las siguientes opciones:
   - Seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - Compruebe que **el cuadro** Actividades contiene **Mostrar resultados para todas las actividades**.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. En los resultados, haga clic en la **columna Actividad** para ordenar los resultados y busque **entradas set-mailbox.**

5. Seleccione una actividad en los resultados para abrir el menú desplegable de detalles. Debe ver los detalles de cada registro de auditoría para determinar si la actividad está relacionada con el reenvío de correo electrónico:
   - **ObjectId:** el valor de alias del buzón que se modificó.
   - **Parámetros**: _ForwardingSmtpAddress_ indica la dirección de correo electrónico de destino.
   - **UserId:** el usuario que configuró el reenvío de correo electrónico en el buzón en el **campo ObjectId.**

Para obtener más información, vea [Determine who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
