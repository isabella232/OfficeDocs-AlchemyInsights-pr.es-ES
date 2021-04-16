---
title: Problemas con MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810501"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="52573-102">Problemas con Azure MFA</span><span class="sxs-lookup"><span data-stu-id="52573-102">Issues with Azure MFA</span></span>
<span data-ttu-id="52573-103">Hay un par de cosas para comprobar si los usuarios no pueden iniciar sesión con la autenticación multifactor (MFA)</span><span class="sxs-lookup"><span data-stu-id="52573-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="52573-104">Es posible que el usuario afectado se bloquee en Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="52573-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="52573-105">Si ese es el caso, los intentos de autenticación para ese usuario específico se denegarán automáticamente.</span><span class="sxs-lookup"><span data-stu-id="52573-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="52573-106">Siga los pasos de este artículo para desbloquearlos.</span><span class="sxs-lookup"><span data-stu-id="52573-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="52573-107">Si desbloquear el usuario no ha sido de ayuda o no está bloqueado, puede intentar restablecer MFA para el usuario y volverá a realizar el proceso de inscripción.</span><span class="sxs-lookup"><span data-stu-id="52573-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="52573-108">Siga los pasos descritos en este artículo.</span><span class="sxs-lookup"><span data-stu-id="52573-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="52573-109">Si es la primera vez que habilita MFA y los usuarios no pueden iniciar sesión en clientes que no son exploradores, como Outlook, Skype, etc., quizás ADAL (Biblioteca de autenticación de Active Directory) no esté habilitado en su suscripción a O365.</span><span class="sxs-lookup"><span data-stu-id="52573-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="52573-110">En este caso, deberá conectarse a Exchange Online Powershell y ejecutar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="52573-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>