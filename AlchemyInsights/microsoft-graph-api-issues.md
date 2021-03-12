---
title: Problemas con la API de Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716206"
---
# <a name="microsoft-graph-api-issues"></a>Problemas con la API de Microsoft Graph

Este tema también puede aplicarse a desarrolladores que aún usan la API de Graph de Azure AD. Sin embargo, se **recomienda encarecidamente** que use Microsoft Graph para todos los escenarios de administración de directorio, identidad y acceso.

**Problemas de autenticación o autorización**

- Si la aplicación no puede adquirir **tokens** para llamar a Microsoft Graph, elige Problema con obtener una categoría de Microsoft Graph de token de acceso **(autenticación)** para obtener ayuda y soporte técnico más específicos en este tema.
- Si tu aplicación recibe **401 o 403** errores de autorización al llamar a Microsoft Graph, elige la categoría Obtener un error denegado de acceso **(Autorización)** de la API de Microsoft Graph para obtener ayuda y soporte técnico más específicos en este tema.

**Quiero usar Microsoft Graph, pero no sé por dónde empezar**

- [Información general de Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Información general sobre la administración de identidades y acceso en Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introducción a la creación de aplicaciones de Microsoft Graph](https://docs.microsoft.com/graph/)
- **Explorador de Microsoft Graph:** probar las API de Microsoft Graph en el inquilino o en un inquilino de demostración

**Quiero usar Microsoft Graph, pero ¿es compatible con las API de directorio v1.0 que necesito?**

Microsoft Graph es la API recomendada para la administración de directorios, identidades y acceso. Sin embargo, todavía hay algunas diferencias entre lo que es posible en Azure AD Graph y Microsoft Graph. Revise los siguientes artículos, que resaltan las diferencias más actualizadas para ayudarle a elegir:

- [Diferencias de tipo de recurso entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferencias de propiedades entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferencias de métodos entre Azure AD y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**La API que estoy llamando no funciona, ¿dónde puedo hacer más pruebas?**

**Explorador de Microsoft Graph:** pruebe las API de Microsoft Graph en el espacio empresarial o en un inquilino de demostración y consulte también las consultas **de** ejemplo en el Explorador de Microsoft Graph.

**Mi aplicación es demasiado lenta y también se está limitando. ¿Qué mejoras puedo realizar?**

Dependiendo del escenario, hay una variedad de opciones a su disposición para que la aplicación sea más performant y, en algunos casos, menos propensa a ser limitada por el servicio (cuando está realizando demasiadas llamadas).

- [Procedimientos recomendados de Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitudes de procesamiento por lotes](https://docs.microsoft.com/graph/json-batching)
- [Realizar un seguimiento de los cambios a través de la consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Recibir notificaciones de cambios a través de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Guía de limitación](https://docs.microsoft.com/graph/throttling)

**¿Dónde puedo encontrar más información sobre errores y problemas conocidos?**

- [Información de respuesta de error de Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conocidos de Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**¿Dónde puedo comprobar el estado de la disponibilidad y conectividad del servicio?**

La disponibilidad del servicio y la conectividad de los servicios subyacentes a los que se puede tener acceso a través de Microsoft Graph pueden afectar a la disponibilidad general y al rendimiento de Microsoft Graph.

- Para el estado del servicio de Azure Active Directory, compruebe el estado de Los servicios de seguridad **y** identidad que aparecen en la página estado [de Azure](https://azure.microsoft.com/status/).
- Para los servicios de Office que contribuyen a Microsoft Graph, compruebe el estado de los servicios enumerados en el Panel de [mantenimiento del servicio de Office.](https://portal.office.com/adminportal/home#/servicehealth)

Los errores de autorización de Microsoft Graph pueden ser el resultado de varios problemas diferentes, la mayoría de los cuales generan un error 401 o 403. Por ejemplo, lo siguiente puede dar lugar a errores de autenticación:

- [Flujos de adquisición de token de acceso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) incorrectos
- [Ámbitos de permiso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurado
- Ausencia de [consentimiento](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Fin de soporte para la Biblioteca de autenticación de Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)_* _

_*A partir del 30 de junio de 2020**, ya no agregaremos nuevas características a ADAL y Azure AD Graph. Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.

A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.

Las aplicaciones que usan ADAL en versiones existentes del sistema operativo seguirán funcionando después de este tiempo, pero no recibirán ningún soporte técnico *ni actualizaciones de seguridad.*

Es posible que las aplicaciones que usan Azure AD Graph después de este tiempo ya no reciban respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

Se recomienda actualizar a la [biblioteca de autenticación de Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), que tiene las últimas características y actualizaciones de seguridad.

Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes del final de la fecha límite de soporte técnico, lo que garantiza que se beneficiarán de las mejoras de seguridad y características continuas de MSAL.

1. [Leer las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Obtener información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Si necesitas ayuda para comprender cuáles de tus aplicaciones usan ADAL, te recomendamos que revises todo el código fuente de tus aplicaciones y, si procede, te llegues a cualquier proveedor de isv o aplicación. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de AAD Graph**

Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones de [Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Nuestra lista de comprobación para la migración proporciona un punto de inicio](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Le recomendamos que revise todos los códigos fuente de sus aplicaciones y, si procede, se ponga en contacto con cualquier ISV o proveedor de aplicaciones que corresponda. El soporte técnico de Microsoft también puede proporcionarle una lista de todo el uso de AAD Graph en el espacio empresarial.
3. Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. La [referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph. También se proporciona información sobre cómo usar los permisos.
