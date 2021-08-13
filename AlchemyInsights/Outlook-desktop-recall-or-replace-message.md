---
title: Outlook Recuperación de escritorio o reemplazo de un mensaje de correo electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918412"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Recuperar o reemplazar un mensaje de Outlook de correo electrónico

- Como administrador, puede recuperar **mensajes en nombre de los usuarios que usan PowerShell**. No puede recuperar mensajes del Centro de administración.
- Solo puede **recuperar los mensajes que se envían a personas de su organización.** Si el mensaje se envió a una dirección de Gmail, por ejemplo, no puedes recuperarlo.
- Solo puede **recuperar mensajes enviados desde Outlook 2016 en el equipo**. Si un usuario envía un mensaje mediante Outlook para Mac o Outlook en la Web, no puede recuperarlo.

Para recuperar o reemplazar un mensaje de correo electrónico:

1. En el panel de carpetas situado a la izquierda de la Outlook, seleccione la carpeta Elementos enviados.
1. Haga doble clic en el mensaje que desea recuperar para abrirlo.
1. Seleccione la **pestaña** Mensaje y, a continuación, **seleccione Acciones** Recuperar  >  **este mensaje**.
1. Seleccione **Eliminar copias no leídas de este** mensaje o Eliminar copias no leídas y reemplace por un nuevo mensaje y, **a** continuación, **seleccione Aceptar**.
1. Si va a enviar un mensaje de reemplazo, redacte el mensaje y, a continuación, **seleccione Enviar**.
1. El éxito o error de una recuperación de mensajes depende de la configuración del destinatario en Outlook. Para ver los pasos para comprobar la recuperación, vea [este artículo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Buscar y eliminar mensajes de correo electrónico en la organización

- Si no es un administrador global, la cuenta debe agregarse al rol administrador de exhibición de documentos electrónicos o al rol de administración búsqueda de cumplimiento para buscar mensajes. Para eliminar mensajes, deberá unirse al grupo de roles Administración de la organización o al rol de administración Buscar y purgar. Los permisos para estos roles se asignan en el [Centro de seguridad y cumplimiento](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Cree una búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/content-search) para buscar el mensaje que desea eliminar.
- [Conectar a PowerShell del Centro de seguridad y cumplimiento.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Si usa la autenticación multifactor, vea Conectar para Microsoft 365 seguridad y el Centro de cumplimiento de PowerShell mediante la autenticación [multifactor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).