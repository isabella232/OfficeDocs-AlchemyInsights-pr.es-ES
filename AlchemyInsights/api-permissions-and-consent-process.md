---
title: Permisos de API y proceso de consentimiento
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379895"
---
# <a name="api-permissions-and-consent-process"></a>Permisos de API y proceso de consentimiento

Para que su aplicación pueda obtener acceso a los datos de Microsoft Graph, el usuario o el administrador deben concederle los permisos correctos a través de un proceso de consentimiento. [La referencia de permisos de Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) enumera los permisos asociados con cada conjunto principal de API de Microsoft Graph. También se proporciona información sobre cómo usar los permisos.

**Configurar o actualizar la entidad de servicio**

- [Crear serviceprincipal:](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) en este artículo se muestra cómo crear un nuevo objeto servicePrincipal.
- Crear una entidad de servicio de & de azure AD en el [portal:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) en este artículo se muestra cómo crear una nueva aplicación de Azure Active Directory (Azure AD) y una entidad de servicio que se pueda usar con el control de acceso basado en roles.
- Aplicaciones & de servicio en [Azure AD:](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) en este artículo se describen el registro de aplicaciones, los objetos de aplicación y las entidades de servicio en Azure Active Directory: qué son, cómo se usan y cómo se relacionan entre sí.

**Agregar o actualizar el registro de la aplicación y proporcionar el consentimiento del administrador**

- [Crear un registro de aplicación:](https://docs.microsoft.com/graph/api/application-post-applications) en este artículo se muestra cómo crear un nuevo objeto de aplicación.
- [Actualizar un registro de aplicación: permisos de API:](https://docs.microsoft.com/graph/api/application-update) en este artículo se muestra cómo actualizar las propiedades de un objeto de aplicación.
- [Proporcionar consentimiento de administrador:](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) para el consentimiento de administrador y el consentimiento en general, se requiere que un administrador conceda explícitamente el consentimiento.
- [RBAC (beta):](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) contenedor de administración de roles para definiciones de roles unificadas y asignaciones de roles para proveedores RBAC de Microsoft 365 que admiten varias entidades de seguridad y varios ámbitos en una sola asignación de roles. Esto es diferente del tipo *de recurso rbacApplication.* Microsoft Intune es un ejemplo de un proveedor RBAC de este tipo. Una asignación de roles en Intune puede tener una matriz de entidades de seguridad y una matriz de grupos de ámbito. **Esto está en beta, lo que significa que aún está en desarrollo y no se recomienda su uso en producción.**
