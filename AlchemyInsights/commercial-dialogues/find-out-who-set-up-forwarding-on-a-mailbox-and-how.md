---
title: Descubra quién configura el reenvío en un buzón y cómo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464872"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Descubra quién configura el reenvío en un buzón y cómo

Si se estableció el reenvío externo en un buzón de correo, la actividad se auditará como parte del cmdlet Set-Mailbox. Este es el modo de encontrar la actividad en el registro de auditoría:

1. Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Seleccione **Búsqueda de registro** de auditoría de >  **búsqueda**.
    > [!NOTE]
    > Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.
1. Asegúrese de que **el campo** Actividades está establecido en **Mostrar resultados para todas las actividades** (valor predeterminado). Especifique el intervalo de fechas. No es necesario especificar un nombre de usuario.
1. Seleccione **Buscar**. Las actividades aparecen en **Resultados**.
1. Seleccione **Filtrar resultados** y, a continuación, **escriba Set-mailbox** en el **campo Filtro** de actividad. Esto devuelve todas **las actividades set-mailbox.**
1. Para ver los detalles, seleccione una actividad y, a continuación, **seleccione Más información**. En **Parámetros,** puede ver la dirección de correo electrónico de reenvío que se estableció en el buzón. UserID **representa** el usuario que configura el reenvío externo en el buzón.
Para obtener más información, [vea Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).