---
title: Problemas con vínculos y direcciones URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707899"
---
# <a name="issues-with-links-and-urls"></a>Problemas con vínculos y direcciones URL

Los URI de redirección o las URL de respuesta (ambas expresiones significan lo mismo) son direcciones URL que usa la Plataforma de identidad de Microsoft para devolver tokens solicitados por aplicaciones. Para obtener información acerca de estas URL, vea los siguientes artículos:

- [Flujos de autenticación y escenarios de aplicaciones](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios): información sobre los URI de redirección en la página de **Registro de aplicación** de cada escenario.
- [Restricciones y limitaciones de los URI de redirección o las URL de respuesta](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**No sé cómo registrar los URI de redirección o las URL de respuesta correctas para mi aplicación**

Al iniciar sesión con la aplicación que está desarrollando, si el cuadro de diálogo de inicio de sesión muestra **AADSTS50011: La dirección URL de respuesta especificada en la solicitud no coincide con las direcciones URL de respuesta configuradas para la aplicación <your app ID>**, tendrá que agregar al registro de la aplicación, el URI de redirección que usó el código en la solicitud de token a la Plataforma de identidad de Microsoft.

Para agregar una dirección URL de respuesta, vaya a la pestaña **Autenticación** en la página **Registro de la aplicación** en Azure Portal y agregue una entrada en la sección **Redirigir los URI**. El valor que debe especificar depende del tipo de aplicación que cree, como se describe a continuación:

- Para aplicaciones web y aplicaciones de una sola página, la dirección URL de respuesta es una dirección URL en su aplicación. Vea [Registro de una aplicación de una sola página](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) o [Registrar una aplicación web con Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Para las aplicaciones de escritorio, el valor que debe elegir depende de:
    - la plataforma (es diferente para MacOS, Windows o Linux)
    - la forma en la que adquiere el token (de forma interactiva, con el flujo de código del dispositivo, con Autenticación Integrada de Windows [IWA] o con nombre de usuario y contraseña).
    Para obtener más información, consulte [Aplicaciones de escritorio - Registro de aplicaciones - URI de redirección](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Para las aplicaciones móviles, el URI de redirección depende de:
    - la plataforma (iOS/Android/UWP)
    - la información usada para crear la aplicación, como el id. de agrupación en iOS, o el nombre del paquete y el hash de firma en Android. La aplicación Azure Portal le ayudará. Para obtener más información, consulte [Configuración de la plataforma y URI de redirección](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Las API web y algunos de los métodos silenciosos para adquirir tokens (IWA y nombre de usuario y contraseña) no requieren un URI de redirección.

**He implementado mi aplicación web y al probarla un mensaje me dice que las URL de respuesta no coinciden**

Agregue URI de redirección para todas las ubicaciones en las que implemente la aplicación web. Para obtener más información, consulte [Registrar una aplicación web con Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Agregue el URI de redirección para una ubicación inmediatamente después implementar la aplicación en esa ubicación.

**No puedo registrar suficientes URL de respuesta**

Digamos que usted es un fabricante de software independiente y tiene una o varias direcciones URI de redirección para cada cliente. Quiere migrar de ADAL/Azure AD v1.0 a MSAL/la Plataforma de identidad de Microsoft, pero ha alcanzado el [número máximo de URI de redirección](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Para resolver este problema, [agregue URI de redirección a las entidades de servicio](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) correspondientes a cada uno de los clientes.
