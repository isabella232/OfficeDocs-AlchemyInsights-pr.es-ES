---
title: Permisos y consentimiento de api
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932114"
---
# <a name="api-permissions-and-consent"></a>Permisos y consentimiento de la API

Las aplicaciones que se integran Plataforma de identidad de Microsoft un modelo de autorización que proporciona a los usuarios y administradores control sobre cómo se puede acceder a los datos. La implementación del modelo de autorización se ha actualizado en el punto de conexión Plataforma de identidad de Microsoft usuario. Cambia la forma en que una aplicación debe interactuar con el Plataforma de identidad de Microsoft. [Los permisos y el](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) consentimiento en el punto de conexión Plataforma de identidad de Microsoft cubre los conceptos básicos de este modelo de autorización, incluidos los ámbitos, los permisos y el consentimiento.

El [Azure Active Directory de consentimiento de Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilita el desarrollo de aplicaciones web multiinquilino y cliente nativas. Estas aplicaciones permiten el inicio de sesión por parte de cuentas de usuario de un inquilino de Azure AD que es diferente del donde está registrada la aplicación. También pueden tener acceso a API web como la API de Microsoft Graph (para tener acceso a Azure AD, Intune y servicios en Microsoft 365) y otras API de servicios Microsoft, además de sus propias API web.

