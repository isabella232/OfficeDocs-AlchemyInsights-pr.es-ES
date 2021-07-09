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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339983"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="a1a6c-102">Grupo de retransmisión saliente</span><span class="sxs-lookup"><span data-stu-id="a1a6c-102">Outbound relay pool</span></span>

<span data-ttu-id="a1a6c-103">Microsoft está realizando algunos cambios en la configuración para retransmitir o reenviar correo electrónico a través de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="a1a6c-104">Los mensajes en determinados escenarios se reenvía o se retransmiten Microsoft 365 mediante un grupo de retransmisión especial.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="a1a6c-105">Los mensajes enviados mediante el grupo de retransmisión podrían terminar en la carpeta de correo no deseado del destinatario.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="a1a6c-106">Para obtener más información, vea [Grupos de entrega salientes](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="a1a6c-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="a1a6c-107">Para evitar un escenario con el grupo de retransmisión, asegúrese de que los mensajes reenviados o retransmitido cumplan uno de los siguientes criterios:</span><span class="sxs-lookup"><span data-stu-id="a1a6c-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="a1a6c-108">El remitente saliente es un dominio aceptado del inquilino.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="a1a6c-109">Sender Policy Framework (SPF) pasa cuando el mensaje llega a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="a1a6c-110">DomainKeys Identified Mail (DKIM) en el dominio de remitente P2 pasa cuando el mensaje llega a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="a1a6c-111">Los mensajes que cumplen los criterios anteriores no se retransmiten a través del grupo de retransmisión.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="a1a6c-112">Si el registro MX de su dominio apunta a un servidor local o de terceros, use el filtrado mejorado para asegurarse de que la validación de SPF es correcta para el correo electrónico entrante y evitar el envío de correo electrónico a través del grupo de retransmisión.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="a1a6c-113">**¿Cómo podemos saber si nos afecta el grupo de retransmisión?**</span><span class="sxs-lookup"><span data-stu-id="a1a6c-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="a1a6c-114">Si los correos electrónicos reenviados o retransmitido usan uno de los criterios anteriores, los mensajes no se retransmitirán a través del grupo de retransmisión.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="a1a6c-115">Sin embargo, si un mensaje se envía a través de un grupo de retransmisión, la DIRECCIÓN IP del servidor saliente se encuentra en el intervalo 40.95.0.0/16 y el nombre del servidor saliente incluye **rly** en el nombre.</span><span class="sxs-lookup"><span data-stu-id="a1a6c-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

