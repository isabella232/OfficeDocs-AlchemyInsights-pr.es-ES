---
title: Recuperar los registros de auditoría
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: 6ca61775d18fb5501911fb3334ef499ff1f06a6b42634367eaf546fc322f822c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889663"
---
# <a name="retrieve-the-audit-logs"></a>Recuperar los registros de auditoría

Al abrir por primera vez el registro de auditoría, está vacío. Tiene que realizar una búsqueda para ver el contenido. Aquí le explicamos cómo realizar una búsqueda general de todas las actividades:

1. Realice uno de los pasos siguientes:
   - En el Centro de cumplimiento de Microsoft 365 en <https://compliance.microsoft.com>, vaya a **Soluciones** \>**Auditoría**. O bien, para ir directamente a la página de **Auditoría**, use <https://compliance.microsoft.com/auditlogsearch>.
   - En el portal de Microsoft 365 Defender en <https://security.microsoft.com>, vaya a **Auditoría**. O bien, para ir directamente a la página de **Auditoría**, use <https://sip.security.microsoft.com/auditlogsearch>.

2. En la página de **Auditoría**, compruebe que la pestaña **Búsqueda** está seleccionada y, a continuación, configure las siguientes opciones:
   - **Intervalo de fecha y hora**: seleccione el intervalo de fecha y hora en los cuadros de **Inicio** y **Finalizar**.
   - **Actividades**: compruebe que está seleccionada la opción **Mostrar resultados para todas las actividades**.
   - **Usuarios**: acepte el valor predeterminado en blanco para entregar resultados de todos los usuarios, o introduzca uno o más usuarios.

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página de **Búsqueda de auditoría**.

4. En los resultados, haga clic en **Filtrar resultados** y escriba **Set-Mailbox** en el cuadro de filtro de actividad.

5. Seleccione un registro de auditoría en los resultados. En el control flotante **Detalles**, haga clic en **Más información** para ver más información, como cliente, Usuario que ha realizado una acción, etc.
