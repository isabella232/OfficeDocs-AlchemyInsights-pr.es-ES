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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028771"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificar cuándo se configura el reenvío de correo electrónico externo en buzones de correo

Cuando un Microsoft 365 configura el reenvío de correo electrónico externo en un buzón, la actividad se audita como parte del cmdlet **Set-Mailbox.** Puede ver la actividad mediante la búsqueda del registro de auditoría en el Centro de seguridad & cumplimiento.

1. Inicie sesión en el Centro [Microsoft 365 cumplimiento](https://protection.office.com/).

2. Vaya a la **página Búsqueda de** registro de auditoría  >  **de** búsqueda.

3. Seleccione el intervalo de fechas en **los campos Fecha de** inicio y Fecha **de** finalización. No es necesario especificar un nombre de usuario. Compruebe que **el campo** Actividades está establecido en **Mostrar resultados para todas las actividades**.

4. Haga clic en **Buscar**.

En los resultados, haga clic **en Filtrar resultados** y escriba **Set-Mailbox** en el cuadro de filtro de actividad. Seleccione un registro de auditoría en los resultados. En **el** menú desplegable Detalles, haga clic **en Más información**. Debe ver los detalles de cada registro de auditoría para determinar si la actividad está relacionada con el reenvío de correo electrónico.

- **ObjectId:** el valor de alias del buzón que se modificó.

- **Parámetros**: _ForwardingSmtpAddress_ indica la dirección de correo electrónico de destino.

- **UserId:** el usuario que configuró el reenvío de correo electrónico en el buzón en el **campo ObjectId.**

Para obtener más información, vea [Determine who set up email forwarding for a mailbox](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
