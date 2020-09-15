---
title: Identificar la dirección IP y el cliente en los registros de auditoría
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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668327"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificar la dirección IP y el cliente en los registros de auditoría

La dirección IP que corresponde a una actividad por parte de un usuario o administrador de Microsoft 365 se muestra en los registros de auditoría. También se registra la información del cliente. Estos son los pasos para identificar dicha información

1. Inicie sesión en el [centro de cumplimiento de & de seguridad de Microsoft 365](https://protection.office.com/).

2. Vaya a la **Search**  >  Página de**búsqueda del registro de auditoría** de búsqueda.

   Si está interesado en una actividad específica, selecciónela en la lista **actividades** . Si no es así, se devolverán todas las actividades del usuario seleccionado (configuración predeterminada).

   **Nota**: es posible que algunas actividades no estén disponibles en el menú **actividades** ; sin embargo, estos elementos de auditoría se devolverán si se selecciona **Mostrar resultados para todas las actividades** (configuración predeterminada).

3. Especifique el nombre de usuario en el campo **usuarios** , seleccione el intervalo de fechas adecuado para la actividad y, a continuación, haga clic en **Buscar**.

En los resultados, puede ver la dirección IP de esa actividad en el panel de resultados. Seleccione el registro de auditoría para ver información detallada en **el control flotante** (por ejemplo, el cliente, el usuario que realizó la acción, etc.).

Para obtener más información, consulte [Buscar la dirección IP del equipo usado para obtener acceso a una cuenta en peligro](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
