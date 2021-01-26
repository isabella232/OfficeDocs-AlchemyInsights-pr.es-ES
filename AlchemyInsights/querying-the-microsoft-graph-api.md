---
title: Consulta de la API de Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950779"
---
# <a name="querying-the-microsoft-graph-api"></a>Consulta de la API de Microsoft Graph

Este tema también puede aplicarse a los desarrolladores que aún usan la API de Graph de Azure AD. Sin embargo, se **recomienda usar** Microsoft Graph para todos los escenarios de administración de acceso, identidad y directorio.

**Problemas de autenticación o autorización**

- Si su aplicación no puede adquirir **tokens** para llamar a Microsoft Graph, elija Problema con la obtención de una categoría de Microsoft Graph de token de acceso **(autenticación)** para obtener ayuda y soporte técnico más específicos en este tema.
- Si la aplicación recibe errores de autorización **401 o 403** al llamar a Microsoft Graph, seleccione la categoría obtener un error de acceso denegado **(Autorización)** de la API de Microsoft Graph para obtener ayuda y soporte técnico más específicos en este tema.

**Quiero usar Microsoft Graph, pero no sé por dónde empezar**

Para obtener más información sobre Microsoft Graph, vea:

- [Información general de Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Información general sobre la administración de identidades y acceso en Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introducción a la creación de aplicaciones de Microsoft Graph](https://docs.microsoft.com/graph/)
- **Explorador de Microsoft Graph:** probar las API de Microsoft Graph en el espacio empresarial o en un inquilino de demostración

**Quiero usar Microsoft Graph, pero ¿es compatible con las API de directorio v1.0 que necesito?**

Microsoft Graph es la API recomendada para la administración de directorios, identidades y acceso. Sin embargo, todavía hay algunas diferencias entre lo que es posible en Azure AD Graph y Microsoft Graph. Revise los siguientes artículos, que resaltan las diferencias más recientes para ayudarle en su elección:

- [Diferencias de tipo de recurso entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferencias de propiedades entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferencias de métodos entre Azure AD y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Cuando se consulta el *objeto de* usuario, faltan muchas de sus propiedades**

`GET https://graph.microsoft.com/v1.0/users` solo devuelve 11 propiedades, ya que Microsoft Graph selecciona automáticamente un conjunto predeterminado de propiedades *de* usuario para devolver. Si necesita *otras propiedades de* usuario, use $select para seleccionar las propiedades que necesita la aplicación. Pruébalo primero **en el Explorador de Microsoft Graph.**

**Algunos valores de propiedad de usuario *son nulos* aunque sé que están establecidos**

La explicación más probable es que a la aplicación se le había concedido el *permiso User.ReadBasic.All.* Esto permite a la aplicación leer un conjunto limitado de propiedades de usuario, devolviendo todas las demás propiedades como nulas incluso si se han establecido anteriormente. En su lugar, intente conceder el *permiso User.Read.All* a la aplicación.

Para obtener más información, vea [Permisos de usuario de Microsoft Graph.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Tengo problemas para usar parámetros de consulta de OData para filtrar datos en mis solicitudes**

Aunque Microsoft Graph admite una amplia gama de parámetros de consulta de OData, muchos de esos parámetros no son totalmente compatibles con los servicios de directorio (recursos que heredan de *directoryObject)* en Microsoft Graph. Las mismas limitaciones que estaban presentes en Azure AD Graph persisten en su mayoría en Microsoft Graph:

1. **No se** admite: $count, $search y $filter *valores null* o *no null*
2. **No se admite:**$filter en determinadas propiedades (vea temas de recursos sobre qué propiedades se pueden filtrar)
3. **No se admite:** paginación, filtrado y ordenación al mismo tiempo
4. **No se admite:** filtrado en una relación. Por ejemplo: busque todos los miembros del grupo de ingeniería que están en el Reino Unido.
5. **Compatibilidad parcial:**$orderby *usuario* (solo displayName y userPrincipalName) y *grupo*
6. **Compatibilidad parcial:**$filter (solo admite compatibilidad *con eq*, *startswith* o *,* o *,* y , y limitado cualquier *),*$expand (expandir las relaciones de un solo objeto devuelve todas las relaciones, pero expandir una colección de relaciones de objetos es limitado)

Para obtener más información, vea [Personalizar las respuestas con parámetros de consulta.](https://docs.microsoft.com/graph/query-parameters)

**The API I'm calling doesn't work- where can I do more testing?**

**Explorador de Microsoft Graph:** pruebe las API de Microsoft Graph en su espacio empresarial o en un espacio empresarial de demostración y consulte también las consultas de ejemplo **en** el Explorador de Microsoft Graph.

**Cuando se consultan datos, parece que se obtiene un conjunto de datos incompleto**

Si está consultando una colección (como los *usuarios),* Microsoft Graph usa límites de página del lado servidor para que los resultados siempre se devuelvan con un tamaño de página predeterminado. La aplicación siempre debe esperar pasar por las colecciones devueltas desde el servicio.

Para obtener más información, vea:

- [Procedimientos recomendados de Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginación de los datos de Microsoft Graph en la aplicación](https://docs.microsoft.com/graph/paging)

**Mi aplicación es demasiado lenta y también se está limitando. ¿Qué mejoras puedo realizar?**

Dependiendo de su escenario, hay una variedad de opciones diferentes a su disposición para que la aplicación sea más performant y, en algunos casos, menos propensa a que el servicio las limite (cuando está realizando demasiadas llamadas).

Para más información, vea:

- [Procedimientos recomendados de Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitudes de procesamiento por lotes](https://docs.microsoft.com/graph/json-batching)
- [Seguimiento de cambios a través de la consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Recibir notificaciones de cambios a través de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Guía de limitación](https://docs.microsoft.com/graph/throttling)

**¿Dónde puedo encontrar más información sobre errores y problemas conocidos?**

- [Información de respuesta de error de Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemas conocidos de Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**¿Dónde puedo comprobar el estado de disponibilidad y conectividad del servicio?**

La disponibilidad del servicio y la conectividad de los servicios subyacentes a los que se puede tener acceso a través de Microsoft Graph pueden afectar a la disponibilidad general y al rendimiento de Microsoft Graph.

- Para el estado del servicio de Azure Active Directory, compruebe el estado de seguridad **+ servicios** de identidad que aparecen en la página de estado [de Azure](https://azure.microsoft.com/status/).
- Para los servicios de Office que contribuyen a Microsoft Graph, compruebe el estado de los servicios enumerados en el Panel de estado del servicio [de Office.](https://portal.office.com/adminportal/home#/servicehealth)
