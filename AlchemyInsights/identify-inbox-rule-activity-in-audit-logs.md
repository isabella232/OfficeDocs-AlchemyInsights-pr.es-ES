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
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976882"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificar la actividad de regla de bandeja de entrada en registros de auditoría

Puede usar la búsqueda de registro de auditoría en el Centro de cumplimiento de Microsoft 365 Seguridad & para ver eventos de regla de bandeja de entrada (crear, modificar y eliminar reglas de la bandeja de entrada).

1. Inicie sesión en el Centro [Microsoft 365 cumplimiento](https://protection.office.com/).

2. Vaya a la **página Búsqueda de** registro de auditoría  >  **de** búsqueda.

3. Seleccione el intervalo de fechas en **los campos Fecha de** inicio y Fecha **de** finalización.

4. En **Exchange de buzones** de  correo , compruebe que el campo Actividades está establecido en **New-InboxRule Create/modify/enable/disable inbox rule**.

5. Haga clic en **Buscar**.

En los resultados, seleccione un registro de auditoría. En el menú desplegable de detalles, haga clic **en Más información**. La información sobre la configuración de la regla de bandeja de entrada se muestra en el **campo Parámetros.**

Para obtener más información, vea [Determining if a user created an inbox rule](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
