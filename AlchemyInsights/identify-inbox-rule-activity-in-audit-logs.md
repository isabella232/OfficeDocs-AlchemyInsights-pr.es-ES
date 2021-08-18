---
title: Identificar la actividad de regla de bandeja de entrada en registros de auditoría
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331140"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar la actividad de regla de bandeja de entrada en registros de auditoría

Puede usar la búsqueda de registro de auditoría en el Centro de cumplimiento de Microsoft 365 para ver eventos de regla de bandeja de entrada (crear, modificar y eliminar reglas de bandeja de entrada).

1. Realice uno de los pasos siguientes:
   - En el Centro de cumplimiento de Microsoft 365 <https://compliance.microsoft.com> en , vaya a Auditoría **de** \> **soluciones**. O bien, para ir directamente a la **página Auditoría,** use <https://compliance.microsoft.com/auditlogsearch> .
   - En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Auditar**. O bien, para ir directamente a la **página Auditoría,** use <https://security.microsoft.com/auditlogsearch> .

2. En la **pestaña Búsqueda** de la **página Auditoría,** configure las siguientes opciones:
   - **Intervalo de fecha y hora:** seleccione el intervalo de fecha y hora en los **cuadros** Inicio **y** Fin.
   - **Actividades:** seleccione uno o varios de los siguientes valores:
     - **New-InboxRule Crear regla de bandeja de entrada a partir de Outlook Web App**
     - **Set-InboxRule Modificar regla desde Outlook Web App**.
     - **Actualizar reglas de la bandeja de entrada Outlook cliente**

3. Cuando haya terminado, haga clic en **Buscar**. Las actividades aparecen en la nueva página **De búsqueda auditoría.**

4. Seleccione una actividad en los resultados para abrir el menú desplegable de detalles. La información sobre la configuración de la regla de bandeja de entrada se muestra en el **campo Parámetros.**

Para obtener más información, vea [Determining if a user created an inbox rule](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
