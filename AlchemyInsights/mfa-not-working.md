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
# <a name="issues-with-azure-mfa"></a>Problemas con Azure MFA
Hay un par de cosas para comprobar si los usuarios no pueden iniciar sesión con la autenticación multifactor (MFA)

1. Es posible que el usuario afectado se bloquee en Azure Active Directory Portal. Si ese es el caso, los intentos de autenticación para ese usuario específico se denegarán automáticamente. [Siga los pasos de este artículo para desbloquearlos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si desbloquear el usuario no ha sido de ayuda o no está bloqueado, puede intentar restablecer MFA para el usuario y volverá a realizar el proceso de inscripción. [Siga los pasos descritos en este artículo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Si es la primera vez que habilita MFA y los usuarios no pueden iniciar sesión en clientes que no son exploradores, como Outlook, Skype, etc., quizás ADAL (Biblioteca de autenticación de Active Directory) no esté habilitado en su suscripción a O365. En este caso, deberá conectarse a Exchange Online Powershell y ejecutar este cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*