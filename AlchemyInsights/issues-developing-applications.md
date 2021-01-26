---
title: Problemas con el desarrollo de aplicaciones
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950799"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="89d1b-102">Problemas con el desarrollo de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="89d1b-102">Issues developing applications</span></span>

<span data-ttu-id="89d1b-103">Para solucionar los problemas más comunes al crear aplicaciones de Azure Active Directory (AD), vea los artículos siguientes:</span><span class="sxs-lookup"><span data-stu-id="89d1b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="89d1b-104">Tengo problemas para iniciar sesión en las aplicaciones solo con el explorador Chrome</span><span class="sxs-lookup"><span data-stu-id="89d1b-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="89d1b-105">No sé cómo cambiar los valores predeterminados de duración del token para mi aplicación</span><span class="sxs-lookup"><span data-stu-id="89d1b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="89d1b-106">Estoy confuso sobre cómo funciona el consentimiento de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="89d1b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="89d1b-107">No sé cómo conceder permisos a mi aplicación</span><span class="sxs-lookup"><span data-stu-id="89d1b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="89d1b-108">No entiendo la diferencia entre los permisos delegados y los de aplicación</span><span class="sxs-lookup"><span data-stu-id="89d1b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="89d1b-109">\***Fin de soporte para la Biblioteca de autenticación de Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="89d1b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="89d1b-110">A partir del 30 de junio de 2020, ya no agregaremos nuevas características a la Biblioteca de autenticación de Active Directory (ADAL) y a la API de Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="89d1b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="89d1b-111">Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.</span><span class="sxs-lookup"><span data-stu-id="89d1b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="89d1b-112">A partir del 30 de junio de 2022, finalizaremos el soporte para ADAL y Azure AD Graph y dejaremos de ofrecer soporte técnico o actualizaciones de seguridad.</span><span class="sxs-lookup"><span data-stu-id="89d1b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="89d1b-113">Como resultado de esta condición, estas son las implicaciones:</span><span class="sxs-lookup"><span data-stu-id="89d1b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="89d1b-114">Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no recibirán actualizaciones de soporte técnico ni de seguridad.</span><span class="sxs-lookup"><span data-stu-id="89d1b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="89d1b-115">Es posible que, después de este momento, las aplicaciones que usan AAD Graph ya no reciban respuestas del punto de conexión de AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="89d1b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="89d1b-116">_ *Migración de ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="89d1b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="89d1b-117">Si usa aplicaciones de Microsoft, le recomendamos que actualice a la biblioteca de autenticación de Microsoft (MSAL), que tiene las características y actualizaciones de seguridad más recientes.</span><span class="sxs-lookup"><span data-stu-id="89d1b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="89d1b-118">Esta recomendación es en el contexto en el que Microsoft inicia el proceso de migrar sus aplicaciones a MSAL antes de la fecha límite del fin de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="89d1b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="89d1b-119">La migración por parte de Microsoft de sus aplicaciones a MSAL garantiza que las aplicaciones se beneficien de las mejoras en seguridad y características continuas de MSAL.</span><span class="sxs-lookup"><span data-stu-id="89d1b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="89d1b-120">Leer las preguntas más frecuentes de ADAL</span><span class="sxs-lookup"><span data-stu-id="89d1b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="89d1b-121">Obtener información sobre cómo migrar aplicaciones según la plataforma</span><span class="sxs-lookup"><span data-stu-id="89d1b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="89d1b-122">Si necesita ayuda para comprender cuáles de sus aplicaciones usan ADAL, le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier proveedor de software independiente (ISV) o proveedor de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="89d1b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="89d1b-123">El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="89d1b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="89d1b-124">**Migración de AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="89d1b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="89d1b-125">Para las aplicaciones que usan AAD Graph, siga nuestras instrucciones para migrar aplicaciones de AAD Graph a Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="89d1b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="89d1b-126">[Nuestra lista de comprobación para la migración proporciona un punto de inicio](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="89d1b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="89d1b-127">El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="89d1b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="89d1b-128">Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier proveedor de software independiente (ISV) o proveedor de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="89d1b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="89d1b-129">El soporte técnico de Microsoft también puede proporcionarle información sobre el uso de AAD Graph en su espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="89d1b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







