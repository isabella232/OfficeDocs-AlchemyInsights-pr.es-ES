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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098619"
---
# <a name="issues-with-azure-mfa"></a>Problemas con Azure MFA
Hay un par de cosas para comprobar si los usuarios no pueden iniciar sesión con la autenticación multifactor (MFA)

1. Es posible que el usuario afectado se bloquee en Azure Active Directory Portal. Si ese es el caso, los intentos de autenticación para ese usuario específico se denegarán automáticamente. [Siga los pasos de este artículo para desbloquearlos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si desbloquear el usuario no ha sido de ayuda o no está bloqueado, puede intentar restablecer MFA para el usuario y volverá a realizar el proceso de inscripción. [Siga los pasos descritos en este artículo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Si es la primera vez que habilita MFA y los usuarios no pueden iniciar sesión en clientes que no son exploradores, como Outlook, Skype, etc., quizás ADAL (Biblioteca de autenticación de Active Directory) no esté habilitado en su suscripción a O365. En este caso, deberá conectarse a Exchange Online Powershell y ejecutar este cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*