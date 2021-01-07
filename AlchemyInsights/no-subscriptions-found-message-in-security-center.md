---
title: Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768529"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad

Si, al acceder al Centro de seguridad de Microsoft Defender recibe el mensaje «No se han encontrado suscripciones», significa que el Azure Active Directory (AAD) que se empleaba para iniciar sesión en el portal no cuenta con una licencia de ATP de Microsoft Defender.  

Las licencias de Windows E5 y Office E5 son licencias separadas.

Abra un caso de soporte técnico si la licencia se ha comprado pero no se ha aprovisionado en esta instancia de AAD. Hay dos posibilidades: <br/>
-   Experimenta un posible problema de aprovisionamiento de la licencia.<br/>
-   Ha aprovisionado sin ser consciente la licencia a un AAD de Microsoft diferente del que se utiliza para la autenticación en el servicio. 