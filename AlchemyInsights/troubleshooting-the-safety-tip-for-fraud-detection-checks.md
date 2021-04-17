---
title: Solución de problemas de la sugerencia de seguridad para comprobaciones de detección de fraudes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834748"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="9783c-102">Solución de problemas de la sugerencia de seguridad para comprobaciones de detección de fraudes</span><span class="sxs-lookup"><span data-stu-id="9783c-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="9783c-103">Si está recibiendo una sugerencia de seguridad que indica "El remitente ha fallado nuestras comprobaciones de detección de fraude y puede que no sea quien parece ser", el remitente no pudo pasar las comprobaciones de autenticación DKIM o SPF.</span><span class="sxs-lookup"><span data-stu-id="9783c-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="9783c-104">El mejor método para resolver esto es que el remitente se autorice.</span><span class="sxs-lookup"><span data-stu-id="9783c-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="9783c-105">Si el remitente envía en su nombre, debe autorizarlos agregando la dirección IP del remitente al registro SPF.</span><span class="sxs-lookup"><span data-stu-id="9783c-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="9783c-106">Consulta Solución de problemas de la sugerencia de seguridad [roja (sospechosa)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obtener más información sobre las comprobaciones de detección de fraudes.</span><span class="sxs-lookup"><span data-stu-id="9783c-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="9783c-107">Estos son algunos otros vínculos que pueden ayudar:</span><span class="sxs-lookup"><span data-stu-id="9783c-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="9783c-108">Cómo Microsoft usa el marco de directivas de remitente (SPF) para evitar la suplantación de identidad</span><span class="sxs-lookup"><span data-stu-id="9783c-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="9783c-109">Configurar SPF para ayudar a evitar la suplantación de identidad</span><span class="sxs-lookup"><span data-stu-id="9783c-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
