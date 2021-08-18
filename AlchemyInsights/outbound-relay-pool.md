---
title: Grupo de retransmisión saliente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326094"
---
# <a name="outbound-relay-pool"></a>Grupo de retransmisión saliente

Microsoft está realizando algunos cambios en la configuración para retransmitir o reenviar correo electrónico a través de Microsoft 365. Los mensajes en determinados escenarios se reenvía o se retransmiten Microsoft 365 mediante un grupo de retransmisión especial. Los mensajes enviados mediante el grupo de retransmisión podrían terminar en la carpeta de correo no deseado del destinatario. Para obtener más información, vea [Grupos de entrega salientes](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Para evitar un escenario con el grupo de retransmisión, asegúrese de que los mensajes reenviados o retransmitido cumplan uno de los siguientes criterios:

- El remitente saliente es un dominio aceptado del inquilino.
- Sender Policy Framework (SPF) pasa cuando el mensaje llega a Microsoft 365.
- DomainKeys Identified Mail (DKIM) en el dominio de remitente P2 pasa cuando el mensaje llega a Microsoft 365.
 
Los mensajes que cumplen los criterios anteriores no se retransmiten a través del grupo de retransmisión.

Si el registro MX de su dominio apunta a un servidor local o de terceros, use el filtrado mejorado para asegurarse de que la validación de SPF es correcta para el correo electrónico entrante y evitar el envío de correo electrónico a través del grupo de retransmisión.

**¿Cómo podemos saber si nos afecta el grupo de retransmisión?**

Si los correos electrónicos reenviados o retransmitido usan uno de los criterios anteriores, los mensajes no se retransmitirán a través del grupo de retransmisión. Sin embargo, si un mensaje se envía a través de un grupo de retransmisión, la DIRECCIÓN IP del servidor saliente se encuentra en el intervalo 40.95.0.0/16 y el nombre del servidor saliente incluye **rly** en el nombre.

