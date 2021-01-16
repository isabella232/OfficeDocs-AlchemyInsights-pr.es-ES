---
title: Configuración de proxy de aplicación
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876590"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="f3322-102">Configuración de proxy de aplicación</span><span class="sxs-lookup"><span data-stu-id="f3322-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="f3322-103">Para comprender cómo configurar una aplicación proxy de aplicación en Azure AD para exponer las aplicaciones locales a la nube, consulte Cómo configurar una aplicación [proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="f3322-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="f3322-104">El inicio de sesión único (SSO) permite a los usuarios tener acceso a una aplicación sin autenticarse varias veces.</span><span class="sxs-lookup"><span data-stu-id="f3322-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="f3322-105">Permite que la autenticación única se produzca en la nube, en Azure Active Directory, y permite que el servicio o conector suplante al usuario para completar los desafíos de autenticación adicionales de la aplicación.</span><span class="sxs-lookup"><span data-stu-id="f3322-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="f3322-106">Para obtener más información, [vea Cómo configurar el inicio de sesión único en una aplicación proxy de aplicación.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="f3322-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="f3322-107">Use [este artículo para](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) solucionar problemas comunes a los que se enfrentan los usuarios al crear una nueva aplicación proxy de aplicación.</span><span class="sxs-lookup"><span data-stu-id="f3322-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="f3322-108">Si tiene un problema al configurar la autenticación back-end en la aplicación, es posible que tenga que solucionar problemas con las configuraciones de delegación limitada [de Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) para proxy de aplicación o seguir las instrucciones para configurar la aplicación con [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) para resolver el problema.</span><span class="sxs-lookup"><span data-stu-id="f3322-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
