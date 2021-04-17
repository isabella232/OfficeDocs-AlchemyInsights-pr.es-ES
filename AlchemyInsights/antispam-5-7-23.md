---
title: Correo no deseado - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821428"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="7c605-102">Corregir problemas de entrega de correo electrónico para el código de error 5.7.23</span><span class="sxs-lookup"><span data-stu-id="7c605-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="7c605-103">Compruebe el registro DNS de SPF para su dominio en un SPF o un registrador de registros DNS disponibles públicamente en la web.</span><span class="sxs-lookup"><span data-stu-id="7c605-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="7c605-104">Compruebe que Microsoft no identificó el mensaje saliente como correo no deseado y que se enrutó a través del [grupo de entrega de alto riesgo](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="7c605-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="7c605-105">Los mensajes del grupo de entrega de alto riesgo no pasarán comprobaciones de SPF y, por lo tanto, la organización de correo electrónico de destino no aceptará los mensajes.</span><span class="sxs-lookup"><span data-stu-id="7c605-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="7c605-106">Si el problema persiste, es posible que deba ponerse en contacto con el administrador del host de correo al que está intentando enviar correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="7c605-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="7c605-107">Anote el error externo detallado disponible en el mensaje de desbotón.</span><span class="sxs-lookup"><span data-stu-id="7c605-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="7c605-108">Es posible que el soporte técnico de Microsoft no pueda ayudar más.</span><span class="sxs-lookup"><span data-stu-id="7c605-108">Microsoft support may not be able to assist further.</span></span>
