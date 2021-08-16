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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034951"
---
# <a name="fix-tenant-policy-action-override"></a>Corregir directiva de inquilino (invalidación de acción)

Una directiva contra correo no deseado en el inquilino afectó a este mensaje. Para revisar la directiva, haga lo siguiente:

1. Vaya al Centro [de Office 365 seguridad & cumplimiento](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a Directiva de **administración** de amenazas contra correo  >    >  [no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Compruebe si el **origen de directiva** indica lo  **siguiente: Add-Xheader/ModifySubject/Redirect/Delete/No action/ CC message**

    Si es así, en la **pestaña** Personalizado, compruebe la configuración de la directiva que afectó al mensaje. Es posible que la configuración estándar **aplicada** a todos los clientes Exchange Online Protection afectaron al mensaje.

Para obtener más información sobre cómo configurar directivas de filtro de correo no deseado, vea [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
