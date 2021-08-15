---
title: Recuperar o reemplazar un mensaje de correo electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024403"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Recuperar o reemplazar un mensaje de correo electrónico en Microsoft 365

- Solo puede **recuperar los mensajes que se envían a personas de su organización.** Por ejemplo, si el mensaje se envió a una dirección de Gmail, no puedes recuperarlo.
- Solo puede **recuperar los mensajes enviados desde Outlook para el equipo**. Si un usuario envía un mensaje mediante Outlook para Mac o Outlook en la Web, no puede recuperarlo.
- Como administrador de inquilinos, puede recuperar mensajes en nombre de los usuarios mediante **PowerShell** (Para obtener más información, vea: [Buscar y eliminar mensajes de correo electrónico](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- No puede recuperar mensajes del Centro de administración. Desplácese hacia abajo hasta "Buscar y eliminar mensajes de correo electrónico en su organización" para obtener más información.

**Recuperar o reemplazar un mensaje de correo electrónico que envió**

1. En el panel de carpetas situado a la izquierda de la Outlook, elija la carpeta Elementos enviados.
2. Abra el mensaje que desea recuperar. Debe hacer doble clic para abrir el mensaje. Seleccionar el mensaje para que aparezca en el panel de lectura no le permitirá recuperar el mensaje.
3. En la pestaña Mensaje, seleccione **Acciones Recuperar**  >  **este mensaje**.
4. Elija **Eliminar copias no leídas de** este mensaje o Eliminar copias no leídas y reemplace por un nuevo mensaje y, **a** continuación, **seleccione Aceptar**.
5. Si va a enviar un mensaje de reemplazo, redacte el mensaje y, a continuación, **seleccione Enviar**.
6. El éxito o error de una recuperación de mensajes depende de la configuración de los destinatarios en Outlook.

Para obtener más información, incluido cómo comprobar la recuperación, vea Recuperar o reemplazar un mensaje [de correo electrónico que envió](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Para buscar y eliminar mensajes de correo electrónico*** en su organización, es más fácil si es un administrador global. Si no es un administrador global, la cuenta debe agregarse al grupo de roles administrador de exhibición de documentos electrónicos o al rol de administración Búsqueda de cumplimiento. Para eliminar mensajes, deberá unirse al grupo de roles Administración de la organización o al rol de administración Buscar y purgar. Los permisos para estos roles se asignan en el [Centro de seguridad & cumplimiento](https://protection.office.com/).

1. [Cree una búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/content-search) para buscar el mensaje que desea eliminar.
2. [Conectarse a PowerShell del Centro de seguridad y cumplimiento](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Si usa MFA (autenticación multifactor), consulte [Conectar to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
