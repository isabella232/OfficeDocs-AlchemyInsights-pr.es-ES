---
title: Corregir directiva de inquilino (invalidación de acción)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737540"
---
# <a name="fix-tenant-policy-action-override"></a>Corregir directiva de inquilino (invalidación de acción)

Una directiva contra correo no deseado en el inquilino afectó a este mensaje. Para revisar la directiva, haga lo siguiente:

1. Vaya al Centro de seguridad y & seguridad de [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a **Directiva** de administración de amenazas  >    >  [contra correo no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Compruebe si el **origen de directiva** indica lo  **siguiente: Add-Xheader/ModifySubject/Redirect/Delete/No action/ CC message**

    Si es así, en la **pestaña** Personalizado, compruebe la configuración de la directiva que afectó al mensaje. Es posible que  la configuración estándar aplicada a todos los clientes de Exchange Online Protection afectara al mensaje.

Para obtener más información sobre cómo configurar directivas de filtro de correo no deseado, vea [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
