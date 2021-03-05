---
title: Buscar eventos realizados en reglas de bandeja de entrada
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465000"
---
# <a name="find-events-performed-on-inbox-rules"></a>Buscar eventos realizados en reglas de bandeja de entrada

Cuando se crean, cambian o eliminan reglas de la bandeja de entrada, los eventos se registran en el registro de auditoría. Este es el modo de revisarlos:

1. Vaya al Centro [de seguridad y cumplimiento de Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Seleccione Buscar > registro de auditoría.

    > [!NOTE]
    > Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.
1. Seleccione el campo Actividades y busque las actividades del buzón de Exchange y, a continuación, New-InboxRule Crear regla de bandeja de entrada desde Outlook Web App. Cuando haya terminado, haga clic fuera del panel para minimizar el panel Actividades.
1. Especifique el intervalo de fechas y, a continuación, en el campo Usuarios, seleccione el nombre de usuario del usuario que desea investigar. Puede seleccionar más de un usuario a la vez.
1. Seleccione Buscar. Las actividades aparecen en Resultados.
1. Para ver detalles, seleccione una actividad y, a continuación, seleccione Más información. En la sección Parámetros, puede ver el nombre de la regla, las condiciones establecidas y las acciones que realizará la regla.

Para obtener más información, vea Search the Office 365 audit log to troubleshoot common scenarios.