---
title: S/MIME en Outlook en la Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010741"
---
# <a name="encrypt-email-messages-in-outlook"></a>Cifrar mensajes de correo electrónico en Outlook

Microsoft 365 El cifrado de mensajes se basa Microsoft Azure Rights Management (Azure RMS), que forma parte de Azure Information Protection. Si la suscripción incluye Azure Rights Management o Azure Information **Protection,** no es necesario realizar ninguna acción para habilitar o activar manualmente el Servicio de administración de derechos.

En función de los comentarios de los clientes, ya no permitiremos que las reglas de flujo de correo Exchange cifre automáticamente el correo electrónico saliente que contenga cierto tipo de información confidencial en el espacio empresarial de forma predeterminada. En su lugar, proporcionamos instrucciones detalladas sobre cómo puede hacerlo. Para obtener más información sobre cómo crear una regla de transporte para cifrar información confidencial, vea [este artículo](https://aka.ms/OmeEtr).

- Si usa Outlook web (anteriormente **OWA):** al redactar un mensaje de correo electrónico, simplemente haga clic **en Proteger** en OWA. Esto aplicará el permiso "No reenviar". Haga **clic en Cambiar permiso** y elija **Cifrar** para cifrar solo el mensaje.

- Si usa **un** cliente Outlook: para enviar un mensaje cifrado desde Outlook 2013 o 2016, o Outlook 2016 para Mac, seleccione Permisos de opciones y, a continuación, seleccione la opción de protección que   >  necesita.

- Para **cifrar automáticamente todo** el correo electrónico enviado a determinados destinatarios u organizaciones asociadas externas, debe crear una regla de transporte de flujo de correo en el Centro Exchange administración. En este artículo de soporte se proporcionan instrucciones [detalladas.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

