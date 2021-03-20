---
title: Solucionar problemas relacionados con la Autenticación de Azure AD y códigos de error de Autorización (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898385"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Solucionar problemas relacionados con la Autenticación de Azure AD y códigos de error de Autorización (AADSTS)

Para resolver códigos de error de autorización de AAD y de autorización (AADSTS), siga los siguientes pasos recomendados:

1. **Resolver códigos de error en su aplicación**

- Las **especificaciones de OAuth2.0** https://tools.ietf.org/html/rfc6749#section-5.2ofrecen instrucciones para resolver errores que aparezcan durante la autenticación mediante la porción de error de la respuesta de error.

    - **error**: Una cadena de código de error que puede usar para clasificar los tipos de errores que se producen y que se deberían usar para reaccionar ante los errores.
    - El campo **error** tiene varios valores posibles; consulte los vínculos de documentación de protocolo y las especificaciones de OAuth 2.0 para más información sobre errores específicos y cómo reaccionar ante los mismos.

- Aquí tiene una respuesta de error de muestra:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Buscar información del código de error actual**

- Los mensajes y códigos de error están sujetos a cambios. Para obtener información actualizada, consulte la página https://login.microsoftonline.com/error para buscar descripciones, correcciones y algunas sugerencias de soluciones alternativas sobre los errores AADST.
- También puede buscar y solucionar [códigos de error de AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) en el artículo [Códigos de error de autorización y Autenticación de Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Obtener ayuda**

- [Soporte técnico y opciones de ayuda para desarrolladores](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options): si necesita respuesta a una pregunta o ayuda para solucionar un problema que no cubra nuestra documentación, puede que sea conveniente contactar con expertos para obtener ayuda. Este artículo ofrece varias sugerencias para obtener respuestas a las preguntas que le surjan mientras desarrolla aplicaciones que se integren con la Plataforma de identidad de Microsoft.








