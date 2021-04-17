---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821464"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="263a1-102">Corregir problemas de entrega para el código de error 550 5.4.1 Acceso de retransmisión denegado</span><span class="sxs-lookup"><span data-stu-id="263a1-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="263a1-103">Este problema se produce al comprobar si una dirección de correo electrónico es válida para evitar [rebotes](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) al entrar en la red de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="263a1-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="263a1-104">Pruebe a hacer lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="263a1-104">Try the following:</span></span>

1. <span data-ttu-id="263a1-105">Determine si el problema es específico de un dominio completo o de una sola dirección de correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="263a1-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="263a1-106">Dominio completo: a veces es necesario sincronizar el dominio; intente [establecer el dominio en Interno y, a continuación, vuelva a Autoritativo](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="263a1-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="263a1-107">Dirección de correo electrónico única: a veces la dirección debe sincronizarse; cambiar la dirección de proxy smtp y, a continuación, volver a cambiarla puede ser de ayuda.</span><span class="sxs-lookup"><span data-stu-id="263a1-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="263a1-108">Determine si el problema es específico de un grupo o una carpeta pública.</span><span class="sxs-lookup"><span data-stu-id="263a1-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="263a1-109">Para algunos tipos de objeto, es posible que los objetos deba crearse manualmente en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="263a1-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="263a1-110">Si necesita ayuda adicional, abra un vale de soporte técnico y especifique el ámbito del problema (incluido el tipo de objeto al que está enviando) para que podamos ayudarle mejor.</span><span class="sxs-lookup"><span data-stu-id="263a1-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>