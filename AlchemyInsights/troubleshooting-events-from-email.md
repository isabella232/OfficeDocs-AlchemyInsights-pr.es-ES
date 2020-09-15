---
title: Solución de problemas de eventos desde el correo electrónico
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658751"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="9e49a-102">Solución de problemas de eventos desde el correo electrónico</span><span class="sxs-lookup"><span data-stu-id="9e49a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="9e49a-103">Compruebe que la característica está habilitada para el buzón: **Get-EventsFromEmailConfiguration-Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="9e49a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="9e49a-104">Después, consulte los registros de "Eventos desde el correo electrónico" **Export-MailboxDiagnosticLogs <mailbox>-Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="9e49a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="9e49a-105">En los registros de "Eventos desde el correo electrónico", busque el InternetMessageId que coincida con el elemento en el buzón.</span><span class="sxs-lookup"><span data-stu-id="9e49a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="9e49a-106">TrustScore determina si el elemento está o no agregado.</span><span class="sxs-lookup"><span data-stu-id="9e49a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="9e49a-107">Solo se agregarán eventos si TrustScore = "De confianza".</span><span class="sxs-lookup"><span data-stu-id="9e49a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="9e49a-108">TrustScore está determinada por las propiedades SPF, Dkim o Dmarc que aparecen en el encabezado del mensaje.</span><span class="sxs-lookup"><span data-stu-id="9e49a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="9e49a-109">Para ver estas propiedades:</span><span class="sxs-lookup"><span data-stu-id="9e49a-109">To view these properties:</span></span>

<span data-ttu-id="9e49a-110">**Escritorio de Outlook**</span><span class="sxs-lookup"><span data-stu-id="9e49a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="9e49a-111">Abrir el elemento</span><span class="sxs-lookup"><span data-stu-id="9e49a-111">Open the item</span></span>
- <span data-ttu-id="9e49a-112">Archivo -> Propiedades -> Encabezados de Internet</span><span class="sxs-lookup"><span data-stu-id="9e49a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="9e49a-113">o</span><span class="sxs-lookup"><span data-stu-id="9e49a-113">or</span></span>

<span data-ttu-id="9e49a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="9e49a-114">**MFCMapi**</span></span>

- <span data-ttu-id="9e49a-115">Ir al elemento en la bandeja de entrada</span><span class="sxs-lookup"><span data-stu-id="9e49a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="9e49a-116">Buscar PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="9e49a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="9e49a-117">Estas propiedades se determinan y se registran durante el transporte y enrutamiento.</span><span class="sxs-lookup"><span data-stu-id="9e49a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="9e49a-118">Para solucionar problemas adicionales, es posible que tenga que realizar un seguimiento con el Soporte de transporte sobre los errores en SPF, DKIM y DMARC.</span><span class="sxs-lookup"><span data-stu-id="9e49a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>