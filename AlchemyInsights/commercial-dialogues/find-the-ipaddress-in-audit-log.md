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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902277"
---
# <a name="find-the-ip-address-in-audit-log"></a>Buscar la dirección IP en el registro de auditoría

La dirección IP que corresponde a una actividad realizada por un usuario o administrador se muestra en los registros de auditoría. También se registra la información del cliente. A continuación se muestra cómo identificar la dirección IP:

1. Realice una de las siguientes acciones:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está habilitada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.

2. En la **página Auditoría,** compruebe que la **pestaña** Búsqueda está seleccionada y, a continuación, configure las siguientes opciones:
   - **Intervalo de fecha y hora:** seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - **Actividades:** si está interesado en una actividad específica, selecciónelo en la lista; de lo contrario, se devolverá el valor predeterminado **Mostrar** resultados para todas las actividades. Tenga en cuenta que es posible que determinadas actividades no estén disponibles para la selección; sin embargo, esos elementos de auditoría se devolverán si se selecciona **Mostrar resultados para todas las** actividades.
   - **Usuarios:** acepte el valor predeterminado en blanco para devolver resultados para todos los usuarios o escriba uno o varios usuarios.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. En los resultados, haga clic **en Filtrar resultados** y escriba **Set-Mailbox** en el cuadro de filtro de actividad.

5. Seleccione un registro de auditoría en los resultados para abrir **el** control desplegable Detalles.

Para obtener más información, [vea Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
