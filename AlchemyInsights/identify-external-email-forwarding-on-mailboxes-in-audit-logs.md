---
title: Identificar el reenvío de correo electrónico externo en buzones de correo en registros de auditoría
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899901"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar cuándo se configura el reenvío de correo electrónico externo en buzones de correo

Cuando un Microsoft 365 configura el reenvío de correo electrónico externo en un buzón, la actividad se audita como parte del cmdlet **Set-Mailbox.** Puede ver la actividad mediante la búsqueda del registro de auditoría. Este es el modo de hacerlo.

1. Realice uno de los pasos siguientes:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://sip.security.microsoft.com/auditlogsearch> .

2. En la **página Auditoría,** compruebe que la **pestaña** Búsqueda está seleccionada y, a continuación, configure las siguientes opciones:
   - Seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - Compruebe que **el cuadro** Actividades contiene **Mostrar resultados para todas las actividades**.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. En los resultados, haga clic **en Filtrar resultados** y escriba **Set-Mailbox** en el cuadro de filtro de actividad.

5. Seleccione un registro de auditoría en los resultados. En **el** menú desplegable Detalles, haga clic **en Más información**. Debe ver los detalles de cada registro de auditoría para determinar si la actividad está relacionada con el reenvío de correo electrónico.

   - **ObjectId:** el valor de alias del buzón que se modificó.
   - **Parámetros**: _ForwardingSmtpAddress_ indica la dirección de correo electrónico de destino.
   - **UserId:** el usuario que configuró el reenvío de correo electrónico en el buzón en el **campo ObjectId.**

Para obtener más información, vea [Determine who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
