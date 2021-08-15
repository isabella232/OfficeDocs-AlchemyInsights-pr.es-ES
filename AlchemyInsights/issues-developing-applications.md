---
title: Problemas con el desarrollo de aplicaciones
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013441"
---
# <a name="issues-developing-applications"></a>Problemas con el desarrollo de aplicaciones

Para solucionar los problemas más comunes al crear aplicaciones de Azure Active Directory (AD), vea los artículos siguientes:

- [Tengo problemas para iniciar sesión en las aplicaciones solo con el explorador Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [No sé cómo cambiar los valores predeterminados de duración del token para mi aplicación](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Estoy confuso sobre cómo funciona el consentimiento de aplicaciones](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [No sé cómo conceder permisos a mi aplicación](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [No entiendo la diferencia entre los permisos delegados y los de aplicación](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Fin de soporte para la Biblioteca de autenticación de Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)***

- A partir del 30 de junio de 2020, ya no agregaremos nuevas características a la Biblioteca de autenticación de Active Directory (ADAL) y a la API de Azure AD Graph (AAD Graph). Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.

- A partir del 30 de junio de 2022, finalizaremos el soporte para ADAL y Azure AD Graph y dejaremos de ofrecer soporte técnico o actualizaciones de seguridad. Como resultado de esta condición, estas son las implicaciones:

    - Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no recibirán actualizaciones de soporte técnico ni de seguridad.

    - Es posible que, después de este momento, las aplicaciones que usan AAD Graph ya no reciban respuestas del punto de conexión de AAD Graph.

**Migración de ADAL**

Si usa aplicaciones de Microsoft, le recomendamos que actualice a la biblioteca de autenticación de Microsoft (MSAL), que tiene las características y actualizaciones de seguridad más recientes. Esta recomendación es en el contexto en el que Microsoft inicia el proceso de migrar sus aplicaciones a MSAL antes de la fecha límite del fin de soporte técnico. 

La migración por parte de Microsoft de sus aplicaciones a MSAL garantiza que las aplicaciones se beneficien de las mejoras en seguridad y características continuas de MSAL.

1. [Leer las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Obtener información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Si necesita ayuda para comprender cuáles de sus aplicaciones usan ADAL, le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier proveedor de software independiente (ISV) o proveedor de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan AAD Graph, siga nuestras instrucciones para migrar aplicaciones de AAD Graph a Microsoft Graph:

1. [Nuestra lista de comprobación para la migración proporciona un punto de inicio](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier proveedor de software independiente (ISV) o proveedor de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle información sobre el uso de AAD Graph en su espacio empresarial.







