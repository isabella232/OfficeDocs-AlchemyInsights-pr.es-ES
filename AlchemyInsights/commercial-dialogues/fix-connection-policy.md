---
title: Directiva de conexión de corrección
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988226"
---
# <a name="fix-connection-policy"></a>Directiva de conexión de corrección

El correo electrónico se marcó como seguro y se entregó a la bandeja de entrada del usuario porque la dirección IP de envío estaba marcada como segura en la directiva de filtro de conexión. Para revisar la directiva, haga lo siguiente:

1. Vaya al Centro [de Office 365 seguridad & cumplimiento](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a Directiva de **administración** de amenazas contra correo  >    >  [no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. En la **pestaña Personalizado,** seleccione la **directiva de filtro de conexión** y, a continuación, seleccione Editar **directiva**.
3. Revise la **lista de direcciones IP** permitidos. Vea si **Caja fuerte lista** está habilitada.

    > [!NOTE]
    > Microsoft se suscribe a fuentes de terceros de remitentes de confianza. Si **Caja fuerte lista está** habilitada, estos remitentes de confianza no se marcan erróneamente como correo no deseado. Te recomiendo seleccionar esta opción, ya que reducirá el número de falsos positivos (correo bueno que se clasifica como correo no deseado) que recibes.
