---
title: Problemas con una entidad de servicio o recurso
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028093"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemas con una entidad de servicio o recurso

1. Si acaba de empezar, los objetos de entidad de seguridad de aplicación y servicio de [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describen el registro de aplicaciones, los objetos de aplicación y las entidades de servicio en Azure Active Directory: qué son, cómo se usan y cómo se relacionan entre sí. También se presenta un escenario de ejemplo multiinquilino para ilustrar la relación entre el objeto de aplicación de una aplicación y los objetos de entidad de servicio correspondientes.
2. Puede obtener más información sobre la relación entre las aplicaciones y las entidades de servicio mediante la lectura de aplicaciones y objetos de entidad de seguridad de [servicio en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Con la [API de la entidad de](https://docs.microsoft.com/graph/api/resources/serviceprincipal)servicio, puede administrar mediante programación instancias de aplicaciones y controlar lo que una aplicación puede hacer dentro del espacio empresarial.
5. [Tipo de recurso servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) enumera todas las propiedades y métodos para el tipo de recurso servicePrincipal.
6. [Las diferencias de](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) tipo de recurso entre Azure AD Graph y Microsoft Graph resaltan las diferencias entre azure ad Graph y recursos Graph Microsoft. Muestra recursos que tienen nombres diferentes o que no están disponibles; también resalta los recursos disponibles en la versión beta de Microsoft Graph pero no en la versión v1.0.

**Problemas con los usuarios invitados**

- [Inicio rápido:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) agregar usuarios invitados al directorio en Azure Portal muestra cómo agregar un nuevo usuario invitado al directorio de Azure AD a través de Azure Portal, enviar una invitación y ver cómo es el proceso de canje de invitaciones del usuario invitado.
- [Tutorial: Crear flujos de usuario en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) muestra cómo crear algunos flujos de usuario recomendados mediante Azure Portal. Si está buscando información sobre cómo configurar un flujo de credenciales de contraseña de propietario de recursos (ROPC) en la aplicación, consulte Configure the resource owner password credentials flow in Azure AD B2C.
