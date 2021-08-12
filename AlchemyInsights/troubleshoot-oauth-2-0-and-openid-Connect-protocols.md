---
title: Solución de problemas de los protocolos OAuth 2.0 y OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921060"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Solución de problemas de los protocolos OAuth 2.0 y OpenID Connect

Para resolver los problemas de OAuth 2.0 y OpenID Connect, realice los siguientes pasos recomendados:

Consulte los siguientes artículos relacionados con la configuración y la solución de problemas de los protocolos OAuth 2.0 y OpenID Connect:

- [Plataforma de identidad de Microsoft y el flujo del código de autorización de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - En este artículo se describe cómo aprender a programar directamente contra el **flujo de concesión de código (PCKE)** en su aplicación, en cualquier lenguaje.
- [Plataforma de identidad de Microsoft y el flujo de credenciales de cliente de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - En este artículo se describe cómo programar directamente contra el **flujo de credenciales de cliente** en su aplicación.
- [Plataforma de identidad de Microsoft y las Credenciales de contraseña del propietario del recurso (ROPC) de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - En este artículo se describe cómo programar directamente contra el **flujo de ROPC** en su aplicación.
    - La Plataforma de identidad de Microsoft solo admite ROPC para espacios empresariales de Azure AD, y no para cuentas personales. Esto significa que necesita usar un punto de conexión específico para espacio empresarial **(https://login.microsoftonline.com/{TenantId_or_Name})** o el punto de conexión de la **organización)**.
    - Las cuentas personales que se invitan a un espacio empresarial de Azure AD no pueden usar ROPC.
    - Las cuentas que no tengan contraseñas no pueden iniciar sesión a través de ROPC. Para este escenario, le recomendamos que use un flujo diferente para su aplicación.
    - Si los usuarios necesitan usar la [autenticación multifactor (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) para iniciar sesión en la aplicación, serán bloqueados.
    - ROPC no es compatible con los escenarios de [federación de identidades híbridas](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (por ejemplo, Azure AD y ADFS usados para autenticar cuentas locales). Si los usuarios son redirigidos a la página completa de un proveedor de identidad local, Azure AD no podrá probar el nombre de usuario y la contraseña con ese proveedor de identidad. Sin embargo, la [Autenticación de paso a través](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) es compatible con ROPC.
    - Una excepción para un escenario de federación de identidades híbridas sería la siguiente: La directiva de detección del dominio principal con **AllowCloudPasswordValidation** establecida en **TRUE** permitirá que el flujo de ROPC funcione para los usuarios federados cuando la contraseña local esté sincronizada con la nube. Para obtener más información, consulte [Habilitar la autenticación ROPC directa de usuarios federados para aplicaciones heredadas.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Plataforma de identidad de Microsoft y el flujo con derechos delegados de OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - En este artículo se describe cómo programar directamente contra el **flujo con derechos delegados** en su aplicación.
- [Plataforma de identidad de Microsoft y el protocolo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - En este artículo se muestra cómo implementar el protocolo OpenID Connect independientemente del lenguaje y se describe cómo enviar y recibir mensajes de HTTP sin usar ninguna biblioteca de código abierto de Microsoft.

**Tokens de acceso**

[Tokens de acceso a la Plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Obtenga información sobre cómo su API puede validar y usar las notificaciones dentro de un token de acceso. Toda la documentación de este artículo, excepto cuando se indique lo contrario, solo se aplica a los tokens emitidos para las API que haya registrado. No se aplica a los tokens emitidos para las API propiedad de Microsoft, ni esos tokens pueden usarse para validar cómo la Plataforma de identidad de Microsoft emitirá tokens para una API que cree.

**Configuración de aplicaciones**

[Restricciones y limitaciones de URI de redirección (dirección URL de respuesta)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Obtenga información sobre cómo configurar el URI de redirección (dirección URL de respuesta). Un URI de redirección, o dirección URL de respuesta, es la ubicación donde el servidor de autorización envía al usuario una vez que la aplicación se ha autorizado correctamente y se ha concedido un código de autorización o un token de acceso. El servidor de autorización envía el código o token al URI de redirección; por lo que es importante que registre la ubicación correcta como parte del proceso de registro de aplicaciones.

**Aprovisionamiento de aplicaciones**

[Tutorial: Desarrollar y planear el aprovisionamiento de un punto de conexión SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - En este artículo se describe cómo compilar un punto de conexión SCIM e integrarlo con el servicio de aprovisionamiento de AAD.


