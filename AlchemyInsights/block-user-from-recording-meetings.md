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
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019201"
---
# <a name="block-user-from-recording-meetings"></a>Bloquear al usuario para que no grabe reuniones

Si necesita impedir o impedir **que** usuarios específicos graben reuniones de Teams, puede hacerlo a través de la configuración Teams directiva de reunión. En el centro Microsoft Teams administración, desactiva la configuración Permitir grabación **en** la nube en la directiva de reunión asignada a ese usuario. Para obtener más información, vea [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Para validar si un usuario específico tiene permiso o no para registrar Teams reuniones, use el diagnóstico de soporte técnico. Ejecute una nueva consulta de soporte técnico y escriba **Diag: Meeting Recording:** el diagnóstico comprobará la configuración de directiva del usuario especificado y determinará su configuración de directiva. Recuerde que la nueva configuración de directiva puede tardar un par de horas en tener efecto, por lo que si acaba de realizar un cambio, espere unas horas antes de volver a ejecutar el diagnóstico.

Para obtener más información, revise [Activar o desactivar la grabación en la nube.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
