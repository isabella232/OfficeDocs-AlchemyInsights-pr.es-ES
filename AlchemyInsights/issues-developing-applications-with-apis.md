---
title: Problemas de desarrollo de aplicaciones con API
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951929"
---
# <a name="issues-developing-applications-with-apis"></a>Problemas de desarrollo de aplicaciones con API

Para empezar a usar la API de Graph de Azure Active Directory, consulte la guía de inicio rápido de la API de [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) o vea la documentación interactiva de referencia de la API de Azure AD [Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Fin de la compatibilidad con la Biblioteca de autenticación de Azure Active Directory (ADAL) y la API de Azure AD Graph (AAD Graph)**

**A partir del 30 de junio de 2020,** ya no agregaremos nuevas características a ADAL y Azure AD Graph. Seguiremos brindando soporte técnico y actualizaciones de seguridad, pero ya no proporcionaremos actualizaciones de características.

A partir del 30 de junio de **2022,** finalizaremos la compatibilidad con ADAL y Azure AD Graph y ya no proporcionaremos soporte técnico ni actualizaciones de seguridad.

Las aplicaciones que usan ADAL en versiones existentes del sistema operativo seguirán funcionando después de este tiempo, pero no recibirán soporte técnico ni actualizaciones de seguridad.

Es posible que las aplicaciones que usan Azure AD Graph después de este tiempo ya no reciban respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

Se recomienda actualizar a la Biblioteca [de autenticación de Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)que tiene las últimas características y actualizaciones de seguridad.

Si usa aplicaciones de Microsoft, sepa que Microsoft está migrando sus aplicaciones a MSAL antes de la fecha límite de finalización del soporte técnico, lo que garantiza que se beneficiarán de las mejoras continuas de seguridad y características de MSAL.

1. [Lea las preguntas más frecuentes sobre ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Obtenga información sobre cómo migrar aplicaciones por plataforma.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Si necesita ayuda para comprender cuál de las aplicaciones usa ADAL, le recomendamos que revise el código fuente de todas las aplicaciones y, si procede, se informe a los ISV o proveedores de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.

**Migración de Gráfico de AAD**

Para las aplicaciones que usan Azure AD Graph, siga nuestras instrucciones para migrar aplicaciones [de Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Nuestra lista de comprobación de migración proporciona un punto de introducción.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. El portal de registro de aplicaciones de Azure muestra qué aplicaciones usan AAD Graph. Te recomendamos que revises el código fuente de todas las aplicaciones y, si procede, te puedes contactar con cualquier ISV o proveedor de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todo el uso de AAD Graph en su espacio empresarial.
1. Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. La [referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph. También se proporciona información sobre cómo usar los permisos.
