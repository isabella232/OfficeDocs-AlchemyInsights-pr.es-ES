---
title: Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768529"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="0403b-102">Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad</span><span class="sxs-lookup"><span data-stu-id="0403b-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="0403b-103">Si, al acceder al Centro de seguridad de Microsoft Defender recibe el mensaje «No se han encontrado suscripciones», significa que el Azure Active Directory (AAD) que se empleaba para iniciar sesión en el portal no cuenta con una licencia de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="0403b-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="0403b-104">Las licencias de Windows E5 y Office E5 son licencias separadas.</span><span class="sxs-lookup"><span data-stu-id="0403b-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="0403b-105">Abra un caso de soporte técnico si la licencia se ha comprado pero no se ha aprovisionado en esta instancia de AAD.</span><span class="sxs-lookup"><span data-stu-id="0403b-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="0403b-106">Hay dos posibilidades:</span><span class="sxs-lookup"><span data-stu-id="0403b-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="0403b-107">Experimenta un posible problema de aprovisionamiento de la licencia.</span><span class="sxs-lookup"><span data-stu-id="0403b-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="0403b-108">Ha aprovisionado sin ser consciente la licencia a un AAD de Microsoft diferente del que se utiliza para la autenticación en el servicio. </span><span class="sxs-lookup"><span data-stu-id="0403b-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>