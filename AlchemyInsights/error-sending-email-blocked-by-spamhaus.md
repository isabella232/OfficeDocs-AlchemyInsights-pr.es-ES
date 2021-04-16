---
title: Error al enviar correo electrónico bloqueado por SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813741"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a3f6c-102">Error al enviar correo electrónico: host de cliente bloqueado con Spamhaus</span><span class="sxs-lookup"><span data-stu-id="a3f6c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a3f6c-103">La dirección IP que envió el mensaje se encuentra en una lista de bloqueo propiedad de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="a3f6c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a3f6c-104">Entre los motivos de bloqueo de Spamhaus se incluyen cuentas comprometidas, máquinas comprometidas que comparten una dirección IP pública y directivas de proveedor de servicios de Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="a3f6c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a3f6c-105">Las correcciones posibles son:</span><span class="sxs-lookup"><span data-stu-id="a3f6c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a3f6c-106">Para los mensajes entrantes bloqueados donde controla el servidor de correo electrónico de origen, debe determinar la causa y quitar el bloque del sitio web de Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a3f6c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a3f6c-107">Para los mensajes entrantes bloqueados en los que la dirección IP de origen pertenece a otra persona, el propietario de la dirección debe quitar el bloque del sitio web de Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a3f6c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a3f6c-108">Si la dirección IP está en la lista de directivas bloqueados (PBL), el propietario puede asignar una dirección IP estática diferente o quitar la dirección del PBL.</span><span class="sxs-lookup"><span data-stu-id="a3f6c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a3f6c-109">Para los mensajes salientes bloqueados de su dominio conectado a Microsoft, puede recibir este error si los mensajes se enruta a través de un servicio de terceros.</span><span class="sxs-lookup"><span data-stu-id="a3f6c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a3f6c-110">Puede usar una herramienta de búsqueda WHOIS para buscar el propietario de la dirección IP bloqueada.</span><span class="sxs-lookup"><span data-stu-id="a3f6c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
