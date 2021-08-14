---
title: Consulta de la API Graph Microsoft
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923256"
---
# <a name="querying-the-microsoft-graph-api"></a>Consulta de la API Graph Microsoft

Este tema también puede aplicarse a los desarrolladores que aún usan la API de Azure AD Graph usuario. Sin embargo, se **recomienda encarecidamente** que use Microsoft Graph para todos los escenarios de administración de directorio, identidad y acceso.

**Problemas de autenticación o autorización**

- Si la aplicación no puede adquirir **tokens** para llamar a Microsoft Graph, elige Problema con la obtención de un token de acceso **(autenticación)** categoría Microsoft Graph para obtener ayuda y soporte técnico más específicos en este tema.
- Si tu aplicación recibe **401 o 403** errores de autorización al llamar a Microsoft Graph, elige la categoría Obtener un error denegado de acceso **(Autorización)** de la API de Microsoft Graph para obtener ayuda y soporte técnico más específicos en este tema.

**Quiero usar Microsoft Graph, pero no sé por dónde empezar**

Para obtener más información sobre Microsoft Graph, vea:

- [Información general de Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Información general sobre la administración de identidades y acceso en Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introducción a la creación de aplicaciones Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer:** probar las API de Microsoft Graph en el inquilino o en un inquilino de demostración

**Quiero usar Microsoft Graph, pero ¿es compatible con las API de directorio v1.0 que necesito?**

Microsoft Graph es la API recomendada para la administración de directorios, identidades y acceso. Sin embargo, todavía hay algunas diferencias entre lo que es posible en Azure AD Graph y Microsoft Graph. Revise los siguientes artículos, que resaltan las diferencias más actualizadas para ayudarle a elegir:

- [Diferencias de tipo de recurso entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Diferencias de propiedades entre Azure AD Graph y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Diferencias de métodos entre Azure AD y Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Al consultar el *objeto de* usuario, faltan muchas de sus propiedades**

`GET https://graph.microsoft.com/v1.0/users`solo devuelve 11 propiedades, ya que Microsoft Graph selecciona automáticamente un conjunto predeterminado de propiedades *de* usuario para devolver. Si necesita otras *propiedades de* usuario, use $select para elegir las propiedades que necesita la aplicación. Pruébalo en **Microsoft Graph Explorer** primero.

**Algunos valores de propiedad de usuario *son nulos* aunque sé que están establecidos**

La explicación más probable es que a la aplicación se le concedió el *permiso User.ReadBasic.All.* Esto permite a la aplicación leer un conjunto limitado de propiedades de usuario, devolviendo todas las demás propiedades como null incluso si se han establecido anteriormente. Intente conceder a la aplicación el permiso *User.Read.All* en su lugar.

Para obtener más información, [vea Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Tengo problemas para usar parámetros de consulta de OData para filtrar datos en mis solicitudes**

Aunque Microsoft Graph admite una amplia gama de parámetros de consulta OData, muchos de estos parámetros no son totalmente compatibles con los servicios de directorio (recursos que heredan de *directoryObject*) en Microsoft Graph. Las mismas limitaciones que estaban presentes en Azure AD Graph persisten en la mayoría de los casos en Microsoft Graph:

1. **No compatible:**$count, $search y $filter *valores null* o *no*
2. **No se admite**: $filter en determinadas propiedades (vea temas de recursos sobre qué propiedades se pueden filtrar)
3. **No compatible:** paginación, filtrado y ordenación al mismo tiempo
4. **No compatible:** filtrado en una relación. Por ejemplo: busque todos los miembros del grupo de ingeniería que están en el Reino Unido.
5. **Compatibilidad parcial:**$orderby *usuario* (solo displayName y userPrincipalName) y *grupo*
6. **Compatibilidad parcial:**$filter (solo admite *compatibilidad* eq , *startswith* *o* *,* y , y , y limitada cualquier *)*, $expand (expandir las relaciones de un único objeto devuelve todas las relaciones, pero expandir una colección de relaciones de objetos es limitado)

Para obtener más información, vea [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).

**La API que estoy llamando no funciona, ¿dónde puedo hacer más pruebas?**

**Microsoft Graph Explorer:** pruebe las API de Microsoft Graph en el inquilino o en un inquilino de demostración y también consulte las consultas **de** ejemplo en El Explorador de Graph Microsoft.

**Cuando se consultan datos, parece que se obtiene un conjunto de datos incompleto**

Si está consultando una colección (como *usuarios),* Microsoft Graph usa límites de página del lado servidor para que los resultados siempre se devuelvan con un tamaño de página predeterminado. La aplicación siempre debe esperar la página a través de las colecciones devueltas desde el servicio.

Para obtener más información, vea:

- [Procedimientos recomendados Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paginación de los datos de Microsoft Graph en la aplicación](https://docs.microsoft.com/graph/paging)

**Mi aplicación es demasiado lenta y también se está limitando. ¿Qué mejoras puedo realizar?**

Según el escenario, hay una variedad de opciones diferentes a su disposición para que la aplicación sea más performant y, en algunos casos, menos propensa a que el servicio le limite (cuando realiza demasiadas llamadas).

Para más información, vea:

- [Procedimientos recomendados Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Solicitudes de procesamiento por lotes](https://docs.microsoft.com/graph/json-batching)
- [Realizar un seguimiento de los cambios a través de la consulta delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Recibir notificaciones de cambios a través de webhooks](https://docs.microsoft.com/graph/webhooks)
- [Guía de limitación](https://docs.microsoft.com/graph/throttling)

**¿Dónde puedo encontrar más información sobre errores y problemas conocidos?**

- [Información Graph respuesta de error de Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemas conocidos de Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**¿Dónde puedo comprobar el estado de la disponibilidad y conectividad del servicio?**

La disponibilidad del servicio y la conectividad de los servicios subyacentes a los que se puede obtener acceso a través de Microsoft Graph puede afectar a la disponibilidad general y el rendimiento de Microsoft Graph.

- Para Azure Active Directory estado del servicio, compruebe el estado de **seguridad + servicios** de identidad que aparecen en la página estado de [Azure](https://azure.microsoft.com/status/).
- Para Office servicios que contribuyen a Microsoft Graph, compruebe el estado de los servicios enumerados en el Panel de mantenimiento Office [servicio](https://portal.office.com/adminportal/home#/servicehealth).
