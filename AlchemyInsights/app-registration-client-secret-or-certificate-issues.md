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
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemas de certificado o secreto de cliente de registro de aplicaciones

¿Expira el secreto de cliente de aplicación?

Independientemente de cómo se haya creado la aplicación registrada, ya sea a través del proceso de registro estándar en el portal de registro de aplicaciones o si la entidad de servicio se creó en el espacio empresarial mediante el consentimiento de la aplicación, deberá crearse un nuevo secreto de cliente antes de la expiración del actual y actualizarse en el código de aplicación relacionado. El período de validez máximo es de 2 años. Como aviso, el valor secreto debe registrarse, ya que dejará de estar visible después de salir de la página Registros de aplicaciones en el portal. Para obtener más información, vea [Inicio rápido: Registrar una](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplicación en la plataforma de identidades de Microsoft y [Procedimientos recomendados para la plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Para obtener más información, vea [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
