---
title: El correo electrónico de flujo de trabajo no se envía
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072537"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>El correo electrónico de flujo de trabajo no se envía para una SharePoint o biblioteca

1. El correo electrónico de los flujos de trabajo no se envía a todos los usuarios o solo a usuarios específicos, o ve el error El mensaje de correo electrónico no se puede **enviar.** Asegúrese de que el correo electrónico tiene un destinatario válido .

    Compruebe si el usuario existe en el grupo **De** todos los permisos (lista de información de usuario) de esa colección de sitios.  Dirección URL directa de ejemplo: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Si el usuario no existe, asegúrese de que el usuario ha iniciado sesión en la página. 
    - Si es un usuario externo, asegúrese de que su invitación se ha aceptado.
    - Si el usuario existe en el grupo de permisos, asegúrese de que la dirección de correo electrónico es correcta.
    - Si la dirección de correo electrónico de los usuarios no está establecida aquí, cree una alerta de ejemplo para ese usuario que fuerza la sincronización de esa cuenta de usuario de perfiles de usuario de SharePoint a esta colección de sitios.
 
2. El correo electrónico de los flujos de trabajo se envía a los administradores de la colección de sitios, pero no a otros usuarios y ve el error HTTP Prohibido en **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Consulte [Acceso denegado al enviar un correo electrónico a un grupo SharePoint .](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Además, compruebe que la **característica** de colección de sitios del modo de bloqueo de permisos de usuario de acceso limitado no está activa.


## <a name="related-topics"></a>Temas relacionados
¿Quieres probar Microsoft Flow en SharePoint Online?
- [Crear Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint y Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


