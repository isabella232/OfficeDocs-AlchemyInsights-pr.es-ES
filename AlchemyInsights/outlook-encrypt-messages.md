---
title: S/MIME en Outlook en la Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511525"
---
# <a name="encrypt-email-messages-in-outlook"></a>Cifrar mensajes de correo electrónico en Outlook

El cifrado de mensajes de Microsoft 365 se basa en Microsoft Azure Rights Management (Azure RMS), que forma parte de Azure Information Protection. Si su suscripción incluye Azure Rights Management o Azure Information Protection, **no necesita realizar ninguna acción para habilitar o activar manualmente** el servicio Rights Management.

En función de los comentarios de los clientes, ya no se habilitarán las reglas de flujo de correo de Exchange para cifrar automáticamente el correo saliente que contiene determinados tipos de información confidencial en el espacio empresarial de forma predeterminada. En su lugar, proporcionamos instrucciones detalladas sobre cómo puede hacerlo usted mismo. Para obtener más información sobre cómo crear una regla de transporte para cifrar información confidencial, consulte [este artículo](https://aka.ms/OmeEtr).

- Si usa Outlook en la web (anteriormente, **OWA**): al redactar un mensaje de correo electrónico, simplemente haga clic en **proteger** en OWA. Se aplicará el permiso "no reenviar". Haga clic en **Cambiar permiso** y elija **cifrar** para cifrar solo el mensaje.

- Si usa el **cliente de Outlook**: para enviar un mensaje cifrado desde Outlook 2013 o 2016 o Outlook 2016 para Mac, seleccione **Opciones**  >  **permisos**y, a continuación, seleccione la opción de protección que necesite.

- Para **cifrar automáticamente todo el correo electrónico** enviado a determinados destinatarios o organizaciones de asociados externos, debe crear una regla de transporte de flujo de correo en el centro de administración de Exchange. Se proporcionan instrucciones detalladas en [este artículo de soporte técnico](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

