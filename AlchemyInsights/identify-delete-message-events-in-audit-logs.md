---
title: Identificar eventos de eliminar mensajes en registros de auditoría
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630086"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Registros de auditoría de mensajes de correo electrónico eliminados

A partir de enero de 2019, Microsoft activará el registro de auditoría de buzones de forma predeterminada. De lo contrario, para revisar eliminar eventos de mensaje para un usuario específico, debe habilitar manualmente las acciones de eliminación para la auditoría. Si el registro de auditoría de buzones ya está habilitado para su organización o para el usuario específico, siga los pasos siguientes.

1. Inicie sesión en el [Centro Microsoft 365 cumplimiento](https://protection.office.com/)

2. Haga **clic en Búsqueda e investigación** y seleccione Búsqueda de registro de **auditoría.**

3. Seleccione el intervalo de fechas en **los campos Fecha de** inicio y Fecha **de** finalización. Especifique el nombre de usuario del usuario que desea investigar (el usuario que eliminó los elementos). En el **campo Actividades,** seleccione **Mensajes eliminados de la carpeta Elementos eliminados** y **Mensajes movidos a la carpeta Elementos eliminados.**

4. Haga clic en **Buscar**.

En los resultados, seleccione un registro de auditoría. En el menú desplegable de detalles, haga clic **en Más información**. Se muestra información adicional sobre el elemento eliminado (por ejemplo, la línea de asunto y la ubicación del elemento cuando se eliminó) en el **campo AffectedItems.** La **propiedad ClientInfoString** mostrará si la eliminación se produjo en Outlook, Outlook en la Web (anteriormente conocido como Outlook Web App) o en cualquier otro dispositivo.

Para obtener más información, vea [Determine who set up email forwarding for a mailbox](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Nota:** No puede recuperar elementos eliminados con la característica de registro de auditoría. Para recuperar mensajes eliminados en Outlook en la Web, vea [Recuperar elementos eliminados en Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
