---
title: Problemas para desarrollar aplicaciones con API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013477"
---
# <a name="issues-developing-applications-with-apis"></a>Problemas para desarrollar aplicaciones con API

Para empezar a usar la API Azure Active Directory Graph, consulte la guía de inicio rápido de la API de [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) o vea la documentación interactiva de referencia de la API de Azure AD [Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Fin de la compatibilidad con la Azure Active Directory de autenticación (ADAL) y la API de Graph Azure AD (AAD Graph)**

A partir del 30 de junio de **2020,** ya no agregaremos nuevas características a ADAL y Azure AD Graph. Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.

A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.

Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no recibirán actualizaciones de soporte técnico ni de seguridad.

Las aplicaciones que usen Azure AD Graph después de este momento ya no recibirán respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

Se recomienda actualizar a la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tiene las últimas características y actualizaciones de seguridad.

Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes de la fecha límite de finalización del soporte técnico, lo que garantiza que se beneficiarán de las mejoras de características y seguridad continuas de MSAL.

1. [Lea las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Obtenga información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Si necesitas ayuda para comprender cuáles de tus aplicaciones usan ADAL, te recomendamos que revises todo el código fuente de tus aplicaciones y, si procede, te llegues a cualquier proveedor de isv o aplicación. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones de [Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Nuestra lista de comprobación para la migración proporciona un punto de inicio](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier ISV o proveedor de aplicaciones que corresponda. El soporte técnico de Microsoft también puede proporcionarle una lista de todos los Graph de AAD en el espacio empresarial.
1. Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. La [referencia Graph de permisos de](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Microsoft muestra los permisos asociados con cada conjunto principal de API Graph Microsoft. También se proporciona información sobre cómo usar los permisos.
