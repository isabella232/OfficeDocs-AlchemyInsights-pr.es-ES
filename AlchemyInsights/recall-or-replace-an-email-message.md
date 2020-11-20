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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353523"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Recuperar o reemplazar un mensaje de correo electrónico en Microsoft 365

- Solo puede **recuperar los mensajes que se envían a las personas de su organización**. Por ejemplo, si el mensaje se envió a una dirección de gmail, no puede recuperarlo.
- Solo puede **recuperar los mensajes enviados desde Outlook para el equipo**. Si un usuario envía un mensaje con Outlook para Mac o Outlook en la web, no puede recuperarlo.
- Como administrador de inquilinos, puede **recuperar mensajes en nombre de los usuarios mediante PowerShell** (para obtener más información, consulte: [Buscar y eliminar mensajes de correo electrónico](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- No puede recuperar mensajes del centro de administración. Desplácese hacia abajo hasta "buscar y eliminar mensajes de correo electrónico de la organización" para obtener más información.

**Recuperar o reemplazar un mensaje de correo electrónico enviado**

1. En el panel de carpetas de la izquierda de la ventana de Outlook, elija la carpeta elementos enviados.
2. Abra el mensaje que desea recuperar. Debe hacer doble clic para abrir el mensaje. La selección del mensaje para que aparezca en el panel de lectura no le permitirá recuperar el mensaje.
3. En la pestaña mensaje, seleccione **acciones**  >  **recuperar este mensaje**.
4. Elija **eliminar copias no leídas de este mensaje** o **eliminar copias no leídas y reemplazarlas por un nuevo mensaje** y, a continuación, seleccione **Aceptar**.
5. Si va a enviar un mensaje de reemplazo, Redacte el mensaje y, a continuación, seleccione **Enviar**.
6. El éxito o el fracaso de una recuperación de mensajes depende de la configuración de los destinatarios en Outlook.

Para obtener más información, incluido cómo comprobar la recuperación, vea [recuperar o reemplazar un mensaje de correo electrónico enviado](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Para buscar y eliminar mensajes de correo electrónico en su organización_**, es más fácil si es un administrador global. Si no es un administrador global, su cuenta debe agregarse al grupo de roles eDiscovery Manager o al rol de administración de búsqueda de cumplimiento. Para eliminar mensajes, debe unirse al grupo de funciones de administración de la organización o al rol de administración de búsqueda y depuración. Los permisos para estos roles se asignan en el [centro de seguridad & cumplimiento](https://protection.office.com/).

1. [Cree una búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/content-search) para buscar el mensaje que se va a eliminar.
2. [Conéctese al Centro de seguridad y cumplimiento de PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Si usa MFA (multi-factor Authentication), consulte [conectarse a Microsoft 365 Security & el centro de cumplimiento de PowerShell con multi-factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
