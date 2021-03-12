---
title: Enviar un mensaje de correo electrónico proporcionando el id. de mensaje de red
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737420"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Enviar un mensaje de correo electrónico proporcionando el id. de mensaje de red

1. En el **menú desplegable** Nuevo envío, seleccione **Correo** electrónico e **Id. de mensaje de red.**
2. Siga estos pasos para buscar el identificador de mensaje de un mensaje de correo electrónico en Outlook:
    1. Haga doble clic en el mensaje de correo electrónico para abrirlo.
    1. Seleccione **Propiedades del**  >  **archivo**.
    1. Abra el Bloc de notas o un documento de Word en blanco y, a continuación, copie y pegue el contenido encontrado en el cuadro Encabezados de **Internet** en el documento abierto para obtener una mejor visibilidad.
    1. Busque el **campo X-MS-Exchange-Organization-Network-Message-Id.** El valor después de **:** es el identificador que necesita para el envío.
3. En **Destinatarios**, si el correo electrónico aterrizó en la carpeta de correo no deseado para todos los destinatarios de este correo electrónico, elija **Seleccionar todo**. Si no es así, seleccione solo el usuario que ha notificado el problema.
4. En **Motivo del** envío , si selecciona Debería haber sido bloqueado , especifique si el mensaje debe haber sido bloqueado como **Correo** no deseado, **Suplantación** de identidad o **Malware** y, a continuación, **seleccione Enviar**. 

Para obtener más información, vea [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).
