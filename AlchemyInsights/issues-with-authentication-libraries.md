---
title: Problemas con las bibliotecas de autenticación
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028021"
---
# <a name="issues-with-authentication-libraries"></a>Problemas con las bibliotecas de autenticación

1. [Plataforma de identidad de Microsoft bibliotecas de autenticación](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) enumera bibliotecas de software intermedio y cliente compatibles con Microsoft.
2. La Biblioteca de autenticación de Microsoft (MSAL) admite varios flujos [de](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) autenticación para su uso en distintos escenarios de aplicación.
3. Para autenticar y adquirir tokens, inicializa una nueva aplicación cliente pública o confidencial en el código. Puedes establecer varias opciones de configuración al inicializar la aplicación cliente en la Biblioteca de autenticación de Microsoft (MSAL). Para obtener más información, vea [Opciones de configuración de la aplicación](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Fin de la compatibilidad con la Azure Active Directory de autenticación (ADAL) y la API de Graph Azure AD (AAD Graph)**

A partir del 30 de junio de **2020,** ya no agregaremos nuevas características a ADAL y Azure AD Graph. Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.

A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.

Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no *recibirán actualizaciones de soporte técnico ni de seguridad*.

Las aplicaciones que usen Azure AD Graph después de este momento ya no recibirán respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

Se recomienda actualizar a la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tiene las últimas características y actualizaciones de seguridad.

Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes de la fecha límite de finalización del soporte técnico, lo que garantiza que se beneficiarán de las mejoras de seguridad y características continuas de MSAL.

Para obtener más información, vea:

1. [Leer las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Obtener información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Si necesitas ayuda para comprender cuáles de tus aplicaciones usan ADAL, te recomendamos que revises todo el código fuente de tus aplicaciones y, si procede, te llegues a cualquier proveedor de isv o aplicación. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones de [Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Nuestra lista de comprobación de migración proporciona un punto de introducción.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier ISV o proveedor de aplicaciones que corresponda. El soporte técnico de Microsoft también puede proporcionarle una lista de todos los Graph de AAD en el espacio empresarial.
3. Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. La [referencia Graph de permisos de](https://docs.microsoft.com/graph/permissions-reference) Microsoft muestra los permisos asociados con cada conjunto principal de API Graph Microsoft. También se proporciona información sobre cómo usar los permisos.
