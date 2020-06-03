---
title: Solución de problemas de la sugerencia de seguridad para las comprobaciones de detección de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505000"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d5083-102">Solución de problemas de la sugerencia de seguridad para las comprobaciones de detección de fraude</span><span class="sxs-lookup"><span data-stu-id="d5083-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d5083-103">Si está recibiendo una sugerencia de seguridad que dice "el remitente produjo un error en nuestras comprobaciones de detección de fraude y puede no ser quien parece ser", entonces el remitente no ha podido pasar comprobaciones de autenticación DKIM o SPF.</span><span class="sxs-lookup"><span data-stu-id="d5083-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d5083-104">El mejor método para resolver esto es que el remitente autorice a sí mismo.</span><span class="sxs-lookup"><span data-stu-id="d5083-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d5083-105">Si el remitente está enviando en su nombre, debe autorizarlos agregando la dirección IP del remitente a su registro de SPF.</span><span class="sxs-lookup"><span data-stu-id="d5083-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d5083-106">Consulte [solución de problemas de la sugerencia de seguridad en rojo (sospechoso) para las comprobaciones de detección de fraude](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="d5083-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d5083-107">Estos son otros vínculos que pueden ayudarle:</span><span class="sxs-lookup"><span data-stu-id="d5083-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d5083-108">Cómo usa Microsoft el marco de directivas de remitente (SPF) para evitar la suplantación de identidad</span><span class="sxs-lookup"><span data-stu-id="d5083-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d5083-109">Configurar SPF para ayudar a evitar la suplantación de identidad</span><span class="sxs-lookup"><span data-stu-id="d5083-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
