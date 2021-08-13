---
title: La carpeta 1336 RecoverableItems está llena
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061773"
---
# <a name="the-recoverable-items-folder-is-full"></a>La carpeta Elementos recuperables está llena

Para Exchange Online buzones de correo, el límite de almacenamiento predeterminado para la carpeta Elementos recuperables es de 30 GB. El límite de almacenamiento de la carpeta Elementos recuperables se aumenta automáticamente a 100 GB si el buzón se coloca en retención por juicio, retención de exhibición de documentos electrónicos o se asigna a una directiva de retención.

Cuando la carpeta Elementos recuperables alcanza el límite de almacenamiento, la funcionalidad del buzón se ve afectada de las siguientes maneras:

- El usuario no puede eliminar elementos del buzón.

- El asistente para carpetas administradas no puede eliminar elementos basados en la etiqueta de retención o en la configuración de carpetas administradas.

- Para los buzones que tienen habilitada la recuperación de elementos únicos o están en espera, el proceso de protección de página de copia en escritura no puede mantener versiones de elementos editados por el usuario.

- Para los buzones que tienen habilitado el registro de auditoría de buzones de correo, no se pueden guardar entradas de registro de auditoría de buzones en la subcarpeta Auditorías de la carpeta Elementos recuperables.

Para los buzones que no están en espera, los administradores pueden usar el comando en Exchange Online PowerShell para eliminar elementos de la carpeta `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Elementos recuperables. Para obtener más información, consulte los siguientes temas:

- [Búsqueda y eliminación de mensajes](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Para los buzones que están en espera, los administradores deben quitar la retención antes de poder eliminar elementos de la carpeta Elementos recuperables. Para obtener más información, vea Eliminar elementos de la carpeta Elementos recuperables de buzones basados en la [nube en espera.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Para evitar que la carpeta Elementos recuperables se vuelva completa, los administradores pueden aumentar el límite de almacenamiento de la carpeta Elementos recuperables para buzones en espera y configurar una directiva de retención de buzones que mueva los elementos de la carpeta Elementos recuperables al buzón de archivo del usuario. Vea [Aumentar la cuota elementos recuperables para buzones en espera.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
