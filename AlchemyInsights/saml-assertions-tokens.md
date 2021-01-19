---
title: Aserciones SAML (tokens)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884618"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="ffc74-102">Aserciones SAML (tokens)</span><span class="sxs-lookup"><span data-stu-id="ffc74-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="ffc74-103">Los tokens de lenguaje de marcado de aserciones de seguridad (SAML) son representaciones XML de notificaciones.</span><span class="sxs-lookup"><span data-stu-id="ffc74-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="ffc74-104">De forma predeterminada, los tokens SAML que Windows Communication Foundation (WCF) usa en escenarios de seguridad federada se emiten tokens.</span><span class="sxs-lookup"><span data-stu-id="ffc74-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="ffc74-105">Para obtener más información, vea [Notificaciones y tokens SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="ffc74-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="ffc74-106">La plataforma de identidad de Microsoft emite varios tipos de tokens de seguridad en el procesamiento de cada flujo de autenticación.</span><span class="sxs-lookup"><span data-stu-id="ffc74-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="ffc74-107">[La referencia de notificaciones de](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) token SAML describe el formato, las características de seguridad y el contenido de los tokens SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="ffc74-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="ffc74-108">Siga las instrucciones de las [duraciones de token configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) en la plataforma de identidad de Microsoft para comprender cómo configurar las duraciones de token.</span><span class="sxs-lookup"><span data-stu-id="ffc74-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="ffc74-109">Siga los pasos descritos en [este artículo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) para comprender cómo configurar el cifrado de token SAML de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ffc74-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="ffc74-110">En Azure AD, puedes configurar las opciones de firma de certificados y el algoritmo de firma de certificados.</span><span class="sxs-lookup"><span data-stu-id="ffc74-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="ffc74-111">Para obtener más información, vea [opciones avanzadas de firma de certificados en el token SAML para aplicaciones de galería en Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="ffc74-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
