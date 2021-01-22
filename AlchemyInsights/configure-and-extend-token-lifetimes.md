---
title: Configurar y extender la duración de un token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912029"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="2c849-102">Configurar y extender la duración de un token</span><span class="sxs-lookup"><span data-stu-id="2c849-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="2c849-103">Puede especificar la duración de un token de acceso, de SAML o de Id. emitido por la Plataforma de identidad de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c849-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="2c849-104">Establezca la vigencia de los tokens de todas las aplicaciones de su organización, de una aplicación de varios inquilinos (de varias organizaciones) o de una entidad de servicio de seguridad de la organización.</span><span class="sxs-lookup"><span data-stu-id="2c849-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="2c849-105">Para más información, consulte [duraciones de token configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="2c849-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="2c849-106">Para ver ejemplos, consulte [ejemplos de cómo configurar duraciones de token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="2c849-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="2c849-107">Para aprender a configurar la duración y compatibilidad de un token en Azure Active Directory B2C (Azure AD B2C), consulte [Configurar tokens en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="2c849-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="2c849-108">El artículo [Configurar el comportamiento de sesión en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describe los métodos de inicio de sesión único (SSO) empleados en Azure AD B2C y le ayuda a elegir el método de SSO más adecuado para configurar la directiva.</span><span class="sxs-lookup"><span data-stu-id="2c849-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="2c849-109">**¿Cuánto duran los tokens? ¿Durante cuánto tiempo son válidos?**</span><span class="sxs-lookup"><span data-stu-id="2c849-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="2c849-110">Los tokens duran 1 hora y la sesión 24 horas.</span><span class="sxs-lookup"><span data-stu-id="2c849-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="2c849-111">Esto quiere decir que, si no se realizan solicitudes en 24 horas, deberá iniciar sesión de nuevo antes de poder solicitar un nuevo token.</span><span class="sxs-lookup"><span data-stu-id="2c849-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="2c849-112">A partir del 30 de mayo de 2020, ningún nuevo espacio empresarial podrá utilizar la directiva de Duración de tokens configurables para configurar los tokens de sesión y de actualización.</span><span class="sxs-lookup"><span data-stu-id="2c849-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="2c849-113">El desuso tendrá lugar varios meses después, lo que significa que dejaremos de reconocer las directivas de tokens de sesión y de actualización.</span><span class="sxs-lookup"><span data-stu-id="2c849-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="2c849-114">Tras el desuso, todavía podrá configurar las duraciones de token de acceso.</span><span class="sxs-lookup"><span data-stu-id="2c849-114">You can still configure access token lifetimes after the deprecation.</span></span>






