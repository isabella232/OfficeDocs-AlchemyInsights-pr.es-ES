---
title: Configurar y extender la duración de un token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912029"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurar y extender la duración de un token

Puede especificar la duración de un token de acceso, de SAML o de Id. emitido por la Plataforma de identidad de Microsoft. Establezca la vigencia de los tokens de todas las aplicaciones de su organización, de una aplicación de varios inquilinos (de varias organizaciones) o de una entidad de servicio de seguridad de la organización. Para más información, consulte [duraciones de token configurables](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Para ver ejemplos, consulte [ejemplos de cómo configurar duraciones de token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Para aprender a configurar la duración y compatibilidad de un token en Azure Active Directory B2C (Azure AD B2C), consulte [Configurar tokens en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

El artículo [Configurar el comportamiento de sesión en Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describe los métodos de inicio de sesión único (SSO) empleados en Azure AD B2C y le ayuda a elegir el método de SSO más adecuado para configurar la directiva.

**¿Cuánto duran los tokens? ¿Durante cuánto tiempo son válidos?**

Los tokens duran 1 hora y la sesión 24 horas. Esto quiere decir que, si no se realizan solicitudes en 24 horas, deberá iniciar sesión de nuevo antes de poder solicitar un nuevo token.

> [!NOTE]
> A partir del 30 de mayo de 2020, ningún nuevo espacio empresarial podrá utilizar la directiva de Duración de tokens configurables para configurar los tokens de sesión y de actualización. El desuso tendrá lugar varios meses después, lo que significa que dejaremos de reconocer las directivas de tokens de sesión y de actualización. Tras el desuso, todavía podrá configurar las duraciones de token de acceso.






