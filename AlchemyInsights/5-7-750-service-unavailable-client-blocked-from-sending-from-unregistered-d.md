---
title: 1048 5.7.750 servicio no disponible. El cliente bloqueó el envío de dominios no registrados
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
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664259"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="604de-103">5.7.750: se bloqueó el envío de un dominio no registrado</span><span class="sxs-lookup"><span data-stu-id="604de-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="604de-104">El error se produce cuando se envía un gran volumen de mensajes desde dominios no aprovisionados en el espacio empresarial (agregados como dominios aceptados y validados).</span><span class="sxs-lookup"><span data-stu-id="604de-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="604de-105">Para evitar este error, puede usar un conector de flujo de correo basado en certificados donde el dominio del certificado sea un dominio aprovisionado o puede aprovisionar todos los dominios de envío.</span><span class="sxs-lookup"><span data-stu-id="604de-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
