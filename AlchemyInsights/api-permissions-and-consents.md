---
title: Permisos y consentimiento de la API
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951923"
---
# <a name="api-permissions-and-consent"></a>Permisos y consentimiento de la API

Las aplicaciones que se integran con la plataforma de identidad de Microsoft siguen un modelo de autorización que proporciona a los usuarios y administradores el control sobre cómo se puede acceder a los datos. La implementación del modelo de autorización se ha actualizado en el punto de conexión de la plataforma de identidad de Microsoft. Cambia la forma en que una aplicación debe interactuar con la plataforma de identidad de Microsoft. [Los permisos y el consentimiento en el](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) punto de conexión de la plataforma de identidad de Microsoft cubren los conceptos básicos de este modelo de autorización, incluidos los ámbitos, los permisos y el consentimiento.

El [marco de consentimiento de Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita el desarrollo de aplicaciones web multiinquilino y cliente nativo. Estas aplicaciones permiten el inicio de sesión por parte de cuentas de usuario desde un inquilino de Azure AD que es diferente del que tiene registrada la aplicación. Es posible que también necesiten tener acceso a las API web, como la API de Microsoft Graph (para acceder a Azure AD, Intune y los servicios de Microsoft 365) y otras API de servicios Microsoft, además de sus propias API web.

