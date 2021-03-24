---
title: Problemas de certificado o secreto de cliente de registro de aplicaciones
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123198"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="09db7-102">Problemas de certificado o secreto de cliente de registro de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="09db7-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="09db7-103">¿Expira el secreto de cliente de aplicación?</span><span class="sxs-lookup"><span data-stu-id="09db7-103">Application client secret expiring?</span></span>

<span data-ttu-id="09db7-104">Independientemente de cómo se haya creado la aplicación registrada, ya sea a través del proceso de registro estándar en el portal de registro de aplicaciones o si la entidad de servicio se creó en el espacio empresarial mediante el consentimiento de la aplicación, deberá crearse un nuevo secreto de cliente antes de la expiración del actual y actualizarse en el código de aplicación relacionado.</span><span class="sxs-lookup"><span data-stu-id="09db7-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="09db7-105">El período de validez máximo es de 2 años.</span><span class="sxs-lookup"><span data-stu-id="09db7-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="09db7-106">Como aviso, el valor secreto debe registrarse, ya que dejará de estar visible después de salir de la página Registros de aplicaciones en el portal.</span><span class="sxs-lookup"><span data-stu-id="09db7-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="09db7-107">Para obtener más información, vea [Inicio rápido: Registrar una](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplicación en la plataforma de identidades de Microsoft y [Procedimientos recomendados para la plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="09db7-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="09db7-108">Para obtener más información, vea [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="09db7-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
