---
title: Leer los registros de auditoría para eventos eliminados
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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967350"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leer los registros de auditoría para eventos eliminados

Este es el modo de hacerlo:

1. Vaya al Centro [de Office 365 seguridad & cumplimiento](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Seleccione **Búsqueda de registro** de auditoría de  >  [**búsqueda**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Si ve un aviso de que necesita activar la característica, adelante y encándala ahora. Si la característica no está activada, los resultados de la búsqueda no podrán extraer datos de fechas anteriores.
1. Seleccione **Actividades** y, a continuación, **busque Exchange de buzón de correo**. Seleccione las **opciones Mensajes eliminados de la carpeta Elementos eliminados** y **Mensajes movidos a la carpeta Elementos** eliminados. Cuando haya terminado, haga clic fuera del panel para minimizar el **panel** Actividades.
1. Especifique el intervalo de fechas y, a continuación, en el cuadro **Usuarios,** seleccione el nombre de usuario del usuario que desea investigar. Puede seleccionar más de un usuario a la vez.
1. Seleccione **Buscar**. Las actividades aparecen en **Resultados**.
1. Para ver los detalles, seleccione una actividad y, a continuación, **seleccione Más información**. Se muestra información adicional sobre el elemento eliminado, como la línea de asunto y la ubicación del elemento cuando se eliminó, en el **campo AffectedItems.**
    > [!NOTE]
    > No puede restaurar elementos eliminados con la característica de registro de auditoría. Para restaurar elementos eliminados, vea [Recuperar elementos eliminados o correo electrónico en Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Para obtener más información, vea [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).
