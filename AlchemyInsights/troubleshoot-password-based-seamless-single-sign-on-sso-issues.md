---
title: Solucionar problemas de inicio de sesión único (SSO) basado en contraseña
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709504"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="ef57c-102">Solucionar problemas de inicio de sesión único (SSO) basado en contraseña</span><span class="sxs-lookup"><span data-stu-id="ef57c-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="ef57c-103">Para obtener información sobre los conceptos básicos del SSO basado en contraseña, consulte Autenticación basada en [contraseñas con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="ef57c-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="ef57c-104">**Configurar SSO basado en contraseñas**</span><span class="sxs-lookup"><span data-stu-id="ef57c-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="ef57c-105">[Configurar el inicio de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) sesión único basado en contraseña: en este artículo se explica más detalladamente la opción sso basada en contraseña.</span><span class="sxs-lookup"><span data-stu-id="ef57c-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="ef57c-106">Si la aplicación que está agregando requiere una configuración personalizada y necesita usar SSO basado en contraseña, este artículo es para usted.</span><span class="sxs-lookup"><span data-stu-id="ef57c-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="ef57c-107">[Configurar el inicio de sesión único](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) basado en contraseña para aplicaciones de inicio de sesión automático: el proxy de aplicación admite varios modos de inicio de sesión único.</span><span class="sxs-lookup"><span data-stu-id="ef57c-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="ef57c-108">El inicio de sesión basado en contraseña está pensado para aplicaciones que usan una combinación de nombre de usuario y contraseña para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="ef57c-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="ef57c-109">Al configurar el inicio de sesión basado en contraseña para la aplicación, los usuarios deben iniciar sesión en la aplicación local una vez.</span><span class="sxs-lookup"><span data-stu-id="ef57c-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="ef57c-110">Después, Azure Active Directory almacena la información de inicio de sesión y la proporciona automáticamente a la aplicación cuando los usuarios tienen acceso a ella de forma remota.</span><span class="sxs-lookup"><span data-stu-id="ef57c-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="ef57c-111">Ya deberías haber publicado y probado la aplicación con proxy de aplicación.</span><span class="sxs-lookup"><span data-stu-id="ef57c-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="ef57c-112">Si no es así, siga los pasos descritos en Publicar aplicaciones con el proxy de aplicación de [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) y, a continuación, continúe con la configuración de SSO basado en contraseña para aplicaciones pre-instaladas.</span><span class="sxs-lookup"><span data-stu-id="ef57c-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="ef57c-113">Para solucionar problemas de SSO basado en contraseña, consulte Solucionar problemas de inicio de sesión único basado en [contraseña en Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="ef57c-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
