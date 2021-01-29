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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037223"
---
# <a name="issues-with-authentication-libraries"></a>Problemas con las bibliotecas de autenticación

1. [Las bibliotecas de autenticación de](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) la plataforma de identidad de Microsoft enumeran bibliotecas de software intermedio y cliente compatibles con Microsoft.
2. La Biblioteca de autenticación de Microsoft (MSAL) admite varios flujos [de](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) autenticación para su uso en diferentes escenarios de aplicación.
3. Para autenticar y adquirir tokens, inicialice una nueva aplicación cliente pública o confidencial en el código. Puede establecer varias opciones de configuración al inicializar la aplicación cliente en la Biblioteca de autenticación de Microsoft (MSAL). Para obtener más información, vea [Opciones de configuración de la aplicación.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Fin de la compatibilidad con la Biblioteca de autenticación de Azure Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)**

**A partir del 30 de junio de 2020,** ya no agregaremos nuevas características a ADAL y Azure AD Graph. Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.

A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.

Las aplicaciones que usan ADAL en versiones existentes del sistema operativo seguirán funcionando después de este tiempo, pero no recibirán soporte técnico *ni actualizaciones de seguridad.*

Es posible que las aplicaciones que usan Azure AD Graph después de este tiempo ya no reciban respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

Se recomienda actualizar a la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tiene las últimas características y actualizaciones de seguridad.

Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes de la fecha límite de finalización del soporte técnico, lo que garantiza que se beneficiarán de las mejoras continuas de seguridad y características de MSAL.

Para obtener más información, vea:

1. [Leer las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Obtener información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Si necesita ayuda para comprender cuál de las aplicaciones usa ADAL, le recomendamos que revise todo el código fuente de las aplicaciones y, si procede, se informe a los ISV o proveedores de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones de [Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nuestra lista de comprobación de migración proporciona un punto de introducción.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier ISV o proveedor de aplicaciones que corresponda. El soporte técnico de Microsoft también puede proporcionarle una lista de todo el uso de AAD Graph en su espacio empresarial.
3. Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. La [referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph. También se proporciona información sobre cómo usar los permisos.
