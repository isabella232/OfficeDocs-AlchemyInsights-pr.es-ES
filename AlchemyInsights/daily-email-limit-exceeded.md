---
title: Se ha superado el límite de correo electrónico diario. El flujo de trabajo está suspendido.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914668"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Límite de correo electrónico diario excedido. El flujo de trabajo está suspendido.

Este error se puede recibir en los siguientes escenarios:

- Tiene un flujo de trabajo en SharePoint Online que usa el tipo de plataforma de flujo de trabajo SharePoint 2010 SharePoint 2013.
- El flujo de trabajo está configurado para enviar un mensaje de correo electrónico personalizado a más de 200 usuarios a la vez, más de 10 000 destinatarios al día o más de 30 mensajes por minuto.
- Al ejecutar el flujo de trabajo, el mensaje de correo electrónico no se envía y observa el siguiente comportamiento:
    - Para un flujo de trabajo con el SharePoint plataforma de 2013, vaya a la página **Estado del flujo de** trabajo. En la página Estado del flujo de trabajo, **el** estado interno se establece en **Iniciado** y el globo de información muestra No se **puede enviar a un destinatario**.

Para evitar este problema, configure el flujo de trabajo para que envíe mensajes de correo electrónico sin superar [los límites Exchange Online remitente.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Por ejemplo, use una pausa en el flujo de trabajo, envíe el correo electrónico a un grupo de Microsoft 365, un grupo de distribución o un grupo de seguridad habilitado para correo, o envíe el mensaje a menos de 200 destinatarios a la vez.


Para obtener más información, vea el siguiente [artículo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Temas relacionados
- [Crear Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint y Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 