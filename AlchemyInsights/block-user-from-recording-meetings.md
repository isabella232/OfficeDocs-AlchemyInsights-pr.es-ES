---
title: Bloquear al usuario para que no grabe reuniones
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897977"
---
# <a name="block-user-from-recording-meetings"></a>Bloquear al usuario para que no grabe reuniones

Si necesitas impedir o **bloquear que** usuarios específicos graben reuniones de Teams, puedes hacerlo a través de la configuración de la directiva de reunión de Teams. En el Centro de administración de Microsoft Teams, desactiva la configuración Permitir grabación **en** la nube en la directiva de reunión asignada a ese usuario. Para obtener más información, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Para validar si un usuario específico tiene permiso o no para grabar reuniones de Teams, use el diagnóstico de soporte técnico. Ejecute una nueva consulta de soporte técnico y escriba **Diag: Meeting Recording:** el diagnóstico comprobará la configuración de directiva del usuario especificado y determinará su configuración de directiva. Recuerde que la nueva configuración de directiva puede tardar un par de horas en tener efecto, por lo que si acaba de realizar un cambio, espere unas horas antes de volver a ejecutar el diagnóstico.

Para obtener más información, revise [Activar o desactivar la grabación en la nube.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
