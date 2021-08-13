---
title: Mover mensajes de correo electrónico al buzón de archivo
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974974"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mover el correo electrónico al buzón de archivo

Si desea que ejecutemos comprobaciones automatizadas para la configuración mencionada a continuación, seleccione el botón atrás <-- en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que tiene problemas para mover el correo electrónico a su buzón de archivo.

1. Confirme que se **ha habilitado un buzón** de archivo. Si no es así, siga los pasos de [este artículo](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) para habilitar el buzón de archivo.

2. Para archivar mensajes automáticamente en el buzón de  archivo, se debe establecer una etiqueta de retención con la acción Mover a archivo para que se aplique automáticamente a la etiqueta de buzón completo **(predeterminado).** Siga los pasos que se indican aquí para crear la etiqueta: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. A continuación, agregue la **etiqueta Archivo** a la directiva de retención. En el Centro Exchange administración, elija **Directivas** de retención  > agregar la etiqueta Mover a archivo a la directiva > **Guardar**.

4. Ahora, [asigne la directiva de retención](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) al buzón del usuario específico. Se aplicará la misma directiva tanto al **buzón principal** como al **buzón de** archivo.

Es posible que sea necesario forzar al Asistente para carpeta administrada (MFA) para ejecutar y aplicar la nueva configuración al buzón del usuario. Ejecute el siguiente comando mientras está conectado a [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) para iniciar el Asistente para carpetas administradas para un buzón específico:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Para obtener más información sobre cómo configurar una directiva de archivo, vea Configurar una directiva de archivo y [eliminación para buzones.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  