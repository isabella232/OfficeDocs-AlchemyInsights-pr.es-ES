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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568685"
---
# <a name="fix-connection-policy"></a>Directiva de conexión de corrección

El correo electrónico se marcó como seguro y se entregó a la bandeja de entrada del usuario porque la dirección IP de envío estaba marcada como segura en la directiva de filtro de conexión. Para revisar la directiva, haga lo siguiente:

1. Vaya al Centro de seguridad y & seguridad de [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)y, a continuación, vaya a **Directiva** de administración de amenazas  >    >  [contra correo no deseado.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. En la **pestaña Personalizado,** seleccione la **directiva de filtro de conexión** y, a continuación, seleccione Editar **directiva**.
3. Revise la **lista de direcciones IP** permitidos. Vea si **la lista segura** está habilitada.

    > [!NOTE]
    > Microsoft se suscribe a fuentes de terceros de remitentes de confianza. Si **la lista segura** está habilitada, estos remitentes de confianza no se marcan erróneamente como correo no deseado. Te recomiendo seleccionar esta opción, ya que reducirá el número de falsos positivos (correo bueno que se clasifica como correo no deseado) que recibes.
