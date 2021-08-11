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
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951510"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemas de certificado o secreto de cliente de registro de aplicaciones

¿Expira el secreto de cliente de aplicación?

Independientemente de cómo se haya creado la aplicación registrada, ya sea a través del proceso de registro estándar en el portal de registro de aplicaciones o si la entidad de servicio se creó en el espacio empresarial mediante el consentimiento de la aplicación, deberá crearse un nuevo secreto de cliente antes de la expiración del actual y actualizarse en el código de aplicación relacionado. El período de validez máximo es de 2 años. Como aviso, el valor secreto debe registrarse, ya que dejará de estar visible después de salir de la página Registros de aplicaciones en el portal. Para obtener más información, consulta [Inicio rápido: Registrar](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) una aplicación en el Plataforma de identidad de Microsoft [y Procedimientos recomendados para el Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Para obtener más información, vea [Create an Azure AD app & service principal in the portal - Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
