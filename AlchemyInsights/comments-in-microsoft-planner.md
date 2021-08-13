---
title: Comentarios en Microsoft Planner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 0d87d8c9fafe49de02b9c0158144287c77339886cdb910e006296eac73a2c497
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995530"
---
# <a name="comments-in-microsoft-planner"></a>Comentarios en Microsoft Planner

Los comentarios de las tareas de un plan se almacenan en el buzón de Exchange Online para el grupo de Microsoft 365 que está asociado al plan.  Cuando publique un comentario en una tarea, se enviará una notificación por correo electrónico a la bandeja de entrada del grupo y recibirá un correo electrónico para cada comentario subsiguiente que se haga en la tarea.

Estas son algunas respuestas a problemas comunes relacionados con los comentarios:

- **Los usuarios no están recibiendo mensajes de correo electrónico**: los comentarios se envían a la bandeja de entrada del grupo al que pertenece el plan. Para que un usuario reciba los mensajes de correo electrónico del grupo, el grupo debe estar configurado para enviar las conversaciones del grupo a las bandejas de entrada de los miembros.

- **Los comentarios no se guardan**: el usuario que agrega el comentario no tiene permiso para enviar correo electrónico al grupo de Microsoft 365. Lea [Cómo funciona Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) para obtener más información sobre este escenario.

- Se muestra el error **Ya no tiene acceso** o **Los usuarios invitados no pueden agregar comentarios**: los usuarios invitados que no pueden enviar mensajes de correo electrónico a la bandeja de entrada del grupo pueden ver este mensaje. Para resolverlo, asegúrese de que el usuario invitado tiene una dirección de correo electrónico válida.

- **Los usuarios eliminados reciben mensajes de correo electrónico**: Si un usuario envía un comentario sobre una tarea antes de que se elimine del plan, el hilo de correo electrónico incluye al usuario para cada comentario de la tarea.

Para obtener información detallada sobre los comentarios con Microsoft Planner, consulte [Cómo funciona Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) y [Comentar en tareas en Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).
