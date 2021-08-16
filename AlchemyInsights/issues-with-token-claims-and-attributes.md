---
title: Problemas con notificaciones y atributos de token
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012901"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemas con notificaciones y atributos de token

**Actualizar, configurar o quitar notificaciones de token**

1. Al usar Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) puede personalizar el tipo de notificación para la notificación de rol en el token de respuesta que recibe después de autorizar una aplicación.
2. Los desarrolladores de aplicaciones pueden usar notificaciones opcionales en sus aplicaciones de Azure AD para especificar qué notificaciones desean en tokens enviados a su aplicación. Para obtener más información, consulta [Proporcionar notificaciones opcionales a la aplicación.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configurar notificaciones de grupo para aplicaciones con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Si usa el inicio de sesión único sin problemas en la aplicación, vea Personalizar notificaciones emitidas en el [token SAML para aplicaciones empresariales.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Asignación de atributos de notificaciones**

1. Para configurar la directiva de asignación de notificaciones con PowerShell, vea Personalizar notificaciones emitidas en tokens para una aplicación específica en un espacio empresarial [(versión preliminar).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Los atributos de extensión de esquema de directorio proporcionan una forma de almacenar datos adicionales en Azure Active Directory objetos de usuario y otros objetos de directorio, como grupos, detalles de inquilinos, entidades de servicio. Solo se pueden usar atributos de extensión en objetos de usuario para emitir notificaciones a las aplicaciones. [El uso de atributos de extensión de](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) esquema de directorio en notificaciones describe cómo usar atributos de extensión de esquema de directorio para enviar datos de usuario a aplicaciones en notificaciones de token.

Para obtener más información sobre las notificaciones de token, vea:

- [Notificaciones en tokens de acceso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Notificaciones en un id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Notificaciones](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que puede esperar en tokens de identificador y tokens de acceso emitidos por Azure AD B2C
- [Referencia de notificaciones de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
