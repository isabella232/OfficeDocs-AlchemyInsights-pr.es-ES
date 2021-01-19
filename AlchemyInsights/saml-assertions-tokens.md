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
# <a name="saml-assertions-tokens"></a>Aserciones SAML (tokens)

1. Los tokens de lenguaje de marcado de aserciones de seguridad (SAML) son representaciones XML de notificaciones. De forma predeterminada, los tokens SAML que Windows Communication Foundation (WCF) usa en escenarios de seguridad federada se emiten tokens. Para obtener más información, vea [Notificaciones y tokens SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. La plataforma de identidad de Microsoft emite varios tipos de tokens de seguridad en el procesamiento de cada flujo de autenticación. [La referencia de notificaciones de](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) token SAML describe el formato, las características de seguridad y el contenido de los tokens SAML 2.0.
3. Siga las instrucciones de las [duraciones de token configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) en la plataforma de identidad de Microsoft para comprender cómo configurar las duraciones de token.
4. Siga los pasos descritos en [este artículo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) para comprender cómo configurar el cifrado de token SAML de Azure AD.
5. En Azure AD, puedes configurar las opciones de firma de certificados y el algoritmo de firma de certificados. Para obtener más información, vea [opciones avanzadas de firma de certificados en el token SAML para aplicaciones de galería en Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
