---
title: Buscar la dirección IP en el registro de auditoría
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017149"
---
# <a name="find-the-ip-address-in-audit-log"></a>Buscar la dirección IP en el registro de auditoría

1. La dirección IP que corresponde a una actividad realizada por un usuario o administrador se muestra en los registros de auditoría. También se registra la información del cliente. A continuación se muestra cómo identificar la dirección IP:

1. Vaya al Centro [de Office 365 seguridad & cumplimiento](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Seleccione **Búsqueda de registro** de auditoría de  >  **[búsqueda](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está habilitada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.
1. Si está interesado en una actividad específica, selecciónelo en la **lista** Actividades; de lo contrario, de forma predeterminada, se devolverán todas las actividades para el usuario seleccionado. Tenga en cuenta que es posible que ciertas actividades no estén disponibles para su selección en el **menú** Actividades; sin embargo, esos elementos de auditoría se devolverán si se selecciona Mostrar resultados **para** todas las actividades (configuración predeterminada).
1. Especifique el intervalo de fechas y, en el **campo Usuarios,** seleccione el nombre de usuario del usuario que desea investigar.
1. Seleccione **Buscar**. Las actividades aparecen en **Resultados**. Puede ver la dirección IP de cada actividad.
1. Para ver detalles, seleccione una actividad y, a continuación, **seleccione Más información**.

Para obtener más información, vea Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).