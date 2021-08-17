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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313516"
---
# <a name="find-events-performed-on-inbox-rules"></a>Buscar eventos realizados en reglas de bandeja de entrada

Cuando se crean, cambian o eliminan reglas de la bandeja de entrada, los eventos se registran en el registro de auditoría. Este es el modo de revisarlos:

1. Realice una de las siguientes acciones:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

    **Nota:** Si ve un aviso de que necesita activar la auditoría, adelante y encándala ahora. Si esta característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.
1. Seleccione el campo Actividades y busque Exchange de buzón de correo y, a continuación, seleccione New-InboxRule Crear regla de bandeja de entrada desde Outlook Web App. Cuando haya terminado, haga clic fuera del panel para minimizar el panel Actividades.
1. Especifique el intervalo de fechas y, a continuación, en el campo Usuarios, seleccione el nombre de usuario del usuario que desea investigar. Puede seleccionar más de un usuario a la vez.
1. Seleccione Buscar. Las actividades aparecen en Resultados.
1. Para ver detalles, seleccione una actividad y, a continuación, seleccione Más información. En la sección Parámetros, puede ver el nombre de la regla, las condiciones establecidas y las acciones que realizará la regla.

2. En la **pestaña Búsqueda** de la **página Auditoría,** configure las siguientes opciones:
   - **Intervalo de fecha y hora:** seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - **Actividades:** seleccione **New-InboxRule Crear regla de bandeja de entrada desde Outlook Web App**

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. Seleccione una actividad en los resultados para abrir el menú desplegable de detalles. En la **sección Parámetros,** puede ver el nombre de la regla, las condiciones establecidas y las acciones que realizará la regla.

Para obtener más información, vea [Buscar en el registro de auditoría para investigar problemas de soporte técnico comunes.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
