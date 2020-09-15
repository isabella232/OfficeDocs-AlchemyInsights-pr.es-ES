---
title: Correo no deseado 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717378"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corregir problemas de entrega para el código de error 550 5.4.1 acceso de retransmisión denegado

Este problema se produce cuando [se comprueba si una dirección de correo electrónico es válida para evitar que se bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) al entrar en la red de Microsoft. Pruebe a hacer lo siguiente:

1. Determine si el problema es específico de un dominio completo o de una sola dirección de correo electrónico:
    - Dominio completo: a veces, es necesario sincronizar el dominio; Pruebe a [configurar el dominio como interno y, a continuación, de nuevo a autoritario](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Dirección de correo electrónico única: a veces, la dirección debe sincronizarse; cambiar la dirección del proxy SMTP y, a continuación, cambiarla de nuevo puede resultarle útil.
2. Determine si el problema es específico de un grupo o una carpeta pública. Para algunos tipos de objetos, es posible que los objetos deban crearse manualmente en Azure Active Directory.

Si necesita ayuda adicional, abra una incidencia de soporte técnico y especifique el ámbito del problema (incluido el tipo de objeto al que va a enviar) para que podamos ayudarle mejor.