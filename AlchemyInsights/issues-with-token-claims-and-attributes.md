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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "50030003"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="1e4e8-102">Problemas con notificaciones y atributos de token</span><span class="sxs-lookup"><span data-stu-id="1e4e8-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="1e4e8-103">**Actualizar, configurar o quitar notificaciones de token**</span><span class="sxs-lookup"><span data-stu-id="1e4e8-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="1e4e8-104">Con Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD), puede personalizar el tipo de notificación para la notificación de rol en el token de respuesta que recibe después de autorizar una aplicación.</span><span class="sxs-lookup"><span data-stu-id="1e4e8-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="1e4e8-105">Los desarrolladores de aplicaciones pueden usar notificaciones opcionales en sus aplicaciones de Azure AD para especificar qué notificaciones desean en los tokens enviados a su aplicación.</span><span class="sxs-lookup"><span data-stu-id="1e4e8-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="1e4e8-106">Para obtener más información, consulta [Proporcionar notificaciones opcionales a la aplicación.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="1e4e8-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="1e4e8-107">[Configurar notificaciones de grupo para aplicaciones con Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="1e4e8-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="1e4e8-108">Si usa el inicio de sesión único sin problemas en la aplicación, vea personalizar las notificaciones emitidas en el [token SAML para aplicaciones empresariales.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="1e4e8-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="1e4e8-109">**Asignación de atributos de notificaciones**</span><span class="sxs-lookup"><span data-stu-id="1e4e8-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="1e4e8-110">Para configurar la directiva de asignación de notificaciones con PowerShell, vea Personalizar notificaciones emitidas en tokens para una aplicación específica en un inquilino [(versión preliminar).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="1e4e8-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="1e4e8-111">Los atributos de extensión de esquema de directorio proporcionan una forma de almacenar datos adicionales en Azure Active Directory en objetos de usuario y otros objetos de directorio, como grupos, detalles del espacio empresarial, entidades de servicio.</span><span class="sxs-lookup"><span data-stu-id="1e4e8-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="1e4e8-112">Solo se pueden usar atributos de extensión en objetos de usuario para emitir notificaciones a las aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="1e4e8-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="1e4e8-113">[El uso de atributos de extensión de](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) esquema de directorio en notificaciones describe cómo usar atributos de extensión de esquema de directorio para enviar datos de usuario a aplicaciones en notificaciones de token.</span><span class="sxs-lookup"><span data-stu-id="1e4e8-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="1e4e8-114">Para obtener más información sobre las notificaciones de token, vea:</span><span class="sxs-lookup"><span data-stu-id="1e4e8-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="1e4e8-115">Notificaciones en tokens de acceso</span><span class="sxs-lookup"><span data-stu-id="1e4e8-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="1e4e8-116">Notificaciones en un id_token</span><span class="sxs-lookup"><span data-stu-id="1e4e8-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="1e4e8-117">[Notificaciones](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) que puede esperar en tokens de identificador y tokens de acceso emitidos por Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="1e4e8-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="1e4e8-118">Referencia de notificaciones de token SAML</span><span class="sxs-lookup"><span data-stu-id="1e4e8-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
