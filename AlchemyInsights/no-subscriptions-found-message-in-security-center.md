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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544125"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="d8245-102">Mensaje que informa de que no se han encontrado suscripciones en el Centro de seguridad</span><span class="sxs-lookup"><span data-stu-id="d8245-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="d8245-103">Si, al acceder al Centro de seguridad de Microsoft Defender recibe el mensaje "No se han encontrado suscripciones", significa que el Azure Active Directory (AAD) que se empleaba para iniciar sesión en el portal no cuenta con una licencia de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="d8245-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="d8245-104">Las licencias de Windows E5 y Office E5 son licencias separadas.</span><span class="sxs-lookup"><span data-stu-id="d8245-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="d8245-p101">Abra un caso de soporte técnico si la licencia se ha comprado pero no se ha aprovisionado en esta instancia de AAD. Puede que:</span><span class="sxs-lookup"><span data-stu-id="d8245-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="d8245-107">Experimenta un posible problema de aprovisionamiento de la licencia.</span><span class="sxs-lookup"><span data-stu-id="d8245-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="d8245-108">Ha aprovisionado sin ser consciente la licencia a un AAD de Microsoft diferente del que se utiliza para la autenticación en el servicio. </span><span class="sxs-lookup"><span data-stu-id="d8245-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>