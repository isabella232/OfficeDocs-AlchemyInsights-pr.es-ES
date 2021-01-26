---
title: Problemas de desarrollo de aplicaciones con API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951929"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="ef4a8-102">Problemas de desarrollo de aplicaciones con API</span><span class="sxs-lookup"><span data-stu-id="ef4a8-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="ef4a8-103">Para empezar a usar la API de Graph de Azure Active Directory, consulte la guía de inicio rápido de la API de [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) o vea la documentación interactiva de referencia de la API de Azure AD [Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="ef4a8-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="ef4a8-104">**Fin de la compatibilidad con la Biblioteca de autenticación de Azure Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="ef4a8-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="ef4a8-105">**A partir del 30 de junio de 2020,** ya no agregaremos nuevas características a ADAL y Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ef4a8-106">Seguiremos brindando soporte técnico y actualizaciones de seguridad, pero ya no proporcionaremos actualizaciones de características.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="ef4a8-107">A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="ef4a8-108">Las aplicaciones que usan ADAL en versiones existentes del sistema operativo seguirán funcionando después de este tiempo, pero no recibirán soporte técnico ni actualizaciones de seguridad.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="ef4a8-109">Es posible que las aplicaciones que usan Azure AD Graph después de este tiempo ya no reciban respuestas del punto de conexión de Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ef4a8-110">**Migración de ADAL**</span><span class="sxs-lookup"><span data-stu-id="ef4a8-110">**ADAL Migration**</span></span>

<span data-ttu-id="ef4a8-111">Se recomienda actualizar a la Biblioteca [de autenticación de Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que tiene las últimas características y actualizaciones de seguridad.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="ef4a8-112">Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes de la fecha límite de finalización del soporte técnico, lo que garantiza que se beneficiarán de las mejoras continuas de seguridad y características de MSAL.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="ef4a8-113">[Lea las preguntas más frecuentes sobre ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="ef4a8-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ef4a8-114">[Obtenga información sobre cómo migrar aplicaciones por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="ef4a8-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="ef4a8-115">Si necesita ayuda para comprender cuál de las aplicaciones usa ADAL, le recomendamos que revise el código fuente de todas las aplicaciones y, si procede, se informe a los ISV o proveedores de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ef4a8-116">El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="ef4a8-117">**Migración de Gráfico de AAD**</span><span class="sxs-lookup"><span data-stu-id="ef4a8-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="ef4a8-118">Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones [de Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ef4a8-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="ef4a8-119">[Nuestra lista de comprobación de migración proporciona un punto de introducción.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="ef4a8-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="ef4a8-120">El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="ef4a8-121">Te recomendamos que revises el código fuente de todas las aplicaciones y, si procede, te puedes contactar con cualquier ISV o proveedor de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="ef4a8-122">El soporte técnico de Microsoft también puede proporcionarle una lista de todo el uso de AAD Graph en su espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="ef4a8-123">Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="ef4a8-124">La [referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="ef4a8-125">También se proporciona información sobre cómo usar los permisos.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-125">It also provides guidance about how to use the permissions.</span></span>
