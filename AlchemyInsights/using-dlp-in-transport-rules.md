---
title: Usar DLP en reglas de transporte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827233"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="013c1-102">Usar DLP en reglas de transporte</span><span class="sxs-lookup"><span data-stu-id="013c1-102">Using DLP in transport rules</span></span>

<span data-ttu-id="013c1-103">Para integrar la Prevención de pérdida de datos (DLP) en un transporte existente, use la condición "**Si el mensaje contiene... Información confidencial**"en la configuración de la regla de transporte.</span><span class="sxs-lookup"><span data-stu-id="013c1-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="013c1-104">**Para información más detallada, consulte:**</span><span class="sxs-lookup"><span data-stu-id="013c1-104">**For more details, see:**</span></span>

- <span data-ttu-id="013c1-105">Tipos de información confidencial de DLP integrados en las reglas de transporte: [Integrar reglas de información confidencial](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="013c1-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="013c1-106">También puede probar la regla con o sin prueba de directiva con el Modo de prueba en la regla.</span><span class="sxs-lookup"><span data-stu-id="013c1-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="013c1-107">Debería esperar 30 minutos después de crear la regla antes de probarla.</span><span class="sxs-lookup"><span data-stu-id="013c1-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="013c1-108">Consulte [Probar el flujo de correo o las reglas de transporte](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="013c1-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="013c1-109">**Nota**: si está intentando implementar una directiva DLP nueva con las reglas de transporte en el Centro de administración de Exchange, use [directivas DLP en el Centro de seguridad y cumplimiento](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) en su lugar.</span><span class="sxs-lookup"><span data-stu-id="013c1-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
