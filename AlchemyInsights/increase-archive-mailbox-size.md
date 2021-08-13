---
title: 305 Aumentar el tamaño del buzón de archivo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926416"
---
# <a name="increase-the-archive-mailbox-size"></a>Aumentar el tamaño del buzón de archivo


Si desea que ejecutemos comprobaciones automatizadas para la configuración mencionada a continuación, seleccione el botón atrás <-- en la parte superior de esta página y, a continuación, escriba la dirección de correo electrónico del usuario que necesita aumentar el tamaño de su buzón de archivo.

Microsoft 365 limita [el](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) tamaño de los buzones de archivo en función de la licencia asignada a la cuenta de usuario. Cuando el buzón de archivo alcanza el 90 % de su tamaño permitido, el usuario recibe una notificación por correo electrónico. Cuando un buzón de archivo alcanza su límite de tamaño, el usuario no puede mover más elementos al buzón de archivo. Microsoft 365 aumentará el tamaño de un buzón de archivo una vez que se alcance el límite de tamaño. En su lugar, los usuarios pueden realizar las siguientes acciones para liberar espacio en el buzón de archivo:

- Exporte los elementos a un archivo .pst mediante Outlook.

- Elimine elementos del buzón de archivo.

Microsoft 365 proporciona **archivado ilimitado** para Office 365 Enterprise licencias E3 y E5. Un administrador debe habilitar esta característica antes de que el buzón de archivo alcance su tamaño máximo. Cuando se habilita el archivado ilimitado, puede tardar hasta 30 días antes de agregar espacio libre al buzón de archivo. Por lo tanto, se recomienda a los administradores comprobar el espacio libre en el buzón de archivo, lo que permite al usuario seguir usando el buzón de archivo mientras se expande. Para obtener más información, vea [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) y Enable unlimited archiving in [Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Para obtener más información sobre cómo obtener acceso al buzón de archivo desde Outlook, vea Outlook requisitos de acceso a elementos de un archivo [expandido automáticamente.](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) Para configurar una directiva de retención que mueva automáticamente elementos al buzón de archivo, vea Configurar una directiva de archivo y eliminación para buzones de correo de la [Microsoft 365 organización](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Nota:** Los archivos de expansión automática no son compatibles con los buzones principales Exchange 2010.
