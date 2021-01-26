---
title: Permisos y consentimiento de la API
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951923"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="94948-102">Permisos y consentimiento de la API</span><span class="sxs-lookup"><span data-stu-id="94948-102">API permissions and consent</span></span>

<span data-ttu-id="94948-103">Las aplicaciones que se integran con la plataforma de identidad de Microsoft siguen un modelo de autorización que proporciona a los usuarios y administradores el control sobre cómo se puede acceder a los datos.</span><span class="sxs-lookup"><span data-stu-id="94948-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="94948-104">La implementación del modelo de autorización se ha actualizado en el punto de conexión de la plataforma de identidad de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="94948-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="94948-105">Cambia la forma en que una aplicación debe interactuar con la plataforma de identidad de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="94948-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="94948-106">[Los permisos y el consentimiento en el](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) punto de conexión de la plataforma de identidad de Microsoft cubren los conceptos básicos de este modelo de autorización, incluidos los ámbitos, los permisos y el consentimiento.</span><span class="sxs-lookup"><span data-stu-id="94948-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="94948-107">El [marco de consentimiento de Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita el desarrollo de aplicaciones web multiinquilino y cliente nativo.</span><span class="sxs-lookup"><span data-stu-id="94948-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="94948-108">Estas aplicaciones permiten el inicio de sesión por parte de cuentas de usuario desde un inquilino de Azure AD que es diferente del que tiene registrada la aplicación.</span><span class="sxs-lookup"><span data-stu-id="94948-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="94948-109">Es posible que también necesiten tener acceso a las API web, como la API de Microsoft Graph (para acceder a Azure AD, Intune y los servicios de Microsoft 365) y otras API de servicios Microsoft, además de sus propias API web.</span><span class="sxs-lookup"><span data-stu-id="94948-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

