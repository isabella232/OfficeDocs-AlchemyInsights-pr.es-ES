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
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109257"
---
# <a name="saml-assertions-tokens"></a>Aserciones SAML (tokens)

1. Los tokens de lenguaje de marcado de aserciones de seguridad (SAML) son representaciones XML de notificaciones. De forma predeterminada, los tokens SAML Windows Communication Foundation (WCF) en escenarios de seguridad federados se emiten tokens. Para obtener más información, vea [Saml Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. El Plataforma de identidad de Microsoft emite varios tipos de tokens de seguridad en el procesamiento de cada flujo de autenticación. [La referencia de notificaciones de](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) token SAML describe el formato, las características de seguridad y el contenido de los tokens SAML 2.0.
3. Siga las instrucciones de [Configurable token lifetimes in Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.
4. Siga los pasos descritos en [este artículo para](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) comprender cómo configurar el cifrado de tokens SAML de Azure AD.
5. En Azure AD, puede configurar las opciones de firma de certificados y el algoritmo de firma de certificados. Para obtener más información, consulta Opciones avanzadas [de firma de certificados en el token SAML para](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)aplicaciones de galería en Azure Active Directory .
