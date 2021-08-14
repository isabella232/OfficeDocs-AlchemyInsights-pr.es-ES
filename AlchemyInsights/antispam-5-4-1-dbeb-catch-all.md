---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932294"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corregir problemas de entrega para el código de error 550 5.4.1 Acceso de retransmisión denegado

Este problema se produce al comprobar si una dirección de correo electrónico es válida para evitar [rebotes](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) al entrar en la red de Microsoft. Pruebe a hacer lo siguiente:

1. Determine si el problema es específico de un dominio completo o de una sola dirección de correo electrónico:
    - Dominio completo: a veces es necesario sincronizar el dominio; intente [establecer el dominio en Interno y, a continuación, vuelva a Autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Dirección de correo electrónico única: a veces la dirección debe sincronizarse; cambiar la dirección de proxy smtp y, a continuación, volver a cambiarla puede ser de ayuda.
2. Determine si el problema es específico de un grupo o una carpeta pública. Para algunos tipos de objeto, es posible que los objetos deba crearse manualmente en Azure Active Directory.

Si necesita ayuda adicional, abra un vale de soporte técnico y especifique el ámbito del problema (incluido el tipo de objeto al que está enviando) para que podamos ayudarle mejor.