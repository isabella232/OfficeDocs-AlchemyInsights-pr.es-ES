---
title: Identificar la dirección IP y el cliente en registros de auditoría
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a596dd4bed90a0d777dcf19c4c82b41c67fac812
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630302"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar la dirección IP y el cliente en registros de auditoría

La dirección IP que corresponde a una actividad de un Microsoft 365 usuario o administrador se muestra en los registros de auditoría. También se registra la información del cliente. Estos son los pasos para identificar dicha información

1. Inicie sesión en el Centro [Microsoft 365 cumplimiento](https://protection.office.com/).

2. Vaya a la **página Búsqueda de** registro de auditoría  >  **de** búsqueda.

   Si está interesado en una actividad específica, selecciónelo en la **lista** Actividades. Si no es así, se devolverán todas las actividades para el usuario seleccionado (configuración predeterminada).

   **Nota:** Es posible que ciertas actividades no estén disponibles en el **menú** Actividades; sin embargo, esos elementos de auditoría se devolverán si se selecciona **Mostrar** resultados para todas las actividades (configuración predeterminada).

3. Especifique el nombre de usuario en el **campo Usuarios,** seleccione el intervalo de fechas adecuado para la actividad y, a continuación, haga clic en **Buscar**.

En los resultados, puede ver la dirección IP de esa actividad en el panel de resultados. Seleccione el registro de auditoría para ver información detallada en el **control** desplegable Detalles (por ejemplo, Cliente, Usuario que realizó la acción, etc.).

Para obtener más información, vea [Finding the IP address of the computer used to access a compromised account](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
