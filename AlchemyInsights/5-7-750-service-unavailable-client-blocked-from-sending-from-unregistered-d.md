---
title: 1048 5.7.750 Servicio no disponible. Cliente bloqueado para enviar desde dominios no registrados
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774268"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="4d308-103">5.7.750: se bloqueó el envío de un dominio no registrado</span><span class="sxs-lookup"><span data-stu-id="4d308-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="4d308-104">El error se produce cuando se envía un gran volumen de mensajes desde dominios que no se aprovisionan en el espacio empresarial (se agregan como dominios aceptados y se validan).</span><span class="sxs-lookup"><span data-stu-id="4d308-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="4d308-105">Para evitar este error, puede usar un conector de flujo de correo basado en certificados donde el dominio del certificado es un dominio aprovisionado o puede aprovisionar todos los dominios de envío.</span><span class="sxs-lookup"><span data-stu-id="4d308-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="4d308-106">Para obtener más información, vea [Corregir problemas de entrega de correo electrónico para los códigos de error del 5.7.700 al 5.7.750 en Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span><span class="sxs-lookup"><span data-stu-id="4d308-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>