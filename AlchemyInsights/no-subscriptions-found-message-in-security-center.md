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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544125"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad

Si, al acceder al Centro de seguridad de Microsoft Defender recibe el mensaje "No se han encontrado suscripciones", significa que el Azure Active Directory (AAD) que se empleaba para iniciar sesión en el portal no cuenta con una licencia de ATP de Microsoft Defender.  

Las licencias de Windows E5 y Office E5 son licencias separadas.

Abra un caso de soporte técnico si la licencia se ha comprado pero no se ha aprovisionado en esta instancia de AAD. Puede que: <br/>
-   Experimenta un posible problema de aprovisionamiento de la licencia.<br/>
-   Ha aprovisionado sin ser consciente la licencia a un AAD de Microsoft diferente del que se utiliza para la autenticación en el servicio. 