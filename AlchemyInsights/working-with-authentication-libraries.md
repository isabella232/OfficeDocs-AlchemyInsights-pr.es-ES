---
title: Trabajar con bibliotecas de autenticación
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
- "9775"
- "9004342"
ms.openlocfilehash: b667e699e1595b21d80788123de13daffbe79a35b1671e9d35eaa6cd980693db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083103"
---
# <a name="working-with-authentication-libraries"></a>Trabajar con bibliotecas de autenticación

Para resolver el problema de la Biblioteca de autenticación de Microsoft (MSAL), realice los pasos recomendados siguientes:

1. **Trabajar con MSAL**: [Bibliotecas de autenticación de la plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries): este artículo muestra la compatibilidad de la biblioteca de autenticación de Microsoft con varios tipos de aplicación. Incluye vínculos al código fuente de la biblioteca, dónde obtener el paquete para el proyecto de la aplicación y si la biblioteca admite el inicio de sesión de usuario (autenticación), el acceso a las API web protegidas (autorización) o ambos.

2. **Solución de problemas**: MSAL admite varios flujos de autenticación para usarlos en diferentes escenarios de aplicación. Dependiendo de cómo se creó la aplicación cliente, MSAL puede usar uno o varios de los flujos de autenticación admitidos por la plataforma de identidad de Microsoft. Estos flujos pueden producir varios tipos de tokens y códigos de autorización, y requieren diferentes tokens para que funcionen.

3. **Tokens de acceso**: [tokens de acceso a la plataforma de identidad de Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens): obtenga información sobre cómo su API puede validar y usar las notificaciones dentro de un token de acceso. Toda la documentación de este artículo, excepto cuando se indica lo contrario, solo se aplica a los tokens emitidos para las API que haya registrado. No se aplica a los tokens emitidos para las API propiedad de Microsoft, ni puede usarse para validar cómo la plataforma de identidad de Microsoft emitirá tokens para una API que cree.

**Fin del soporte para la Biblioteca de autenticación de Azure Active Directory (ADAL)**

- **A partir del 30 de junio de 2020**, ya no se agregarán nuevas características a ADAL y Azure AD Graph. Seguiremos proporcionando soporte técnico y actualizaciones de seguridad, pero dejaremos de ofrecer actualizaciones de características.
- **A partir del 30 de junio de 2022**, finalizaremos el soporte para ADAL y Azure AD Graph y dejaremos de ofrecer soporte técnico o actualizaciones de seguridad.
- Las aplicaciones que usen ADAL en versiones existentes del SO seguirán funcionando después de este momento, pero no *recibirán actualizaciones de soporte técnico ni de seguridad*.
- Las aplicaciones que usen Azure AD Graph después de este momento ya no recibirán respuestas del punto de conexión de Azure AD Graph.

**Migración de ADAL**

- Le recomendamos que actualice a MSAL, que tiene las características y las actualizaciones de seguridad más recientes.
- Si usa aplicaciones de Microsoft, sepa que Microsoft está en el proceso de migrar sus aplicaciones a MSAL para la fecha límite del fin de soporte técnico, para asegurarse de que se beneficiarán de las mejoras continuas en características y seguridad de MSAL.

1. [Lea las preguntas más frecuentes de ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Obtenga información sobre cómo migrar aplicaciones según la plataforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Si, después de leer la guía de la plataforma de su aplicación, tiene más preguntas, puede publicar en [Preguntas y respuestas de Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) con la etiqueta [azure-ad-adal-deprecation] o abrir un problema en el repositorio de GitHub de la biblioteca. Consulte la sección [Idiomas y marcos](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) del artículo de **información general de MSAL** para ver vínculos al repositorio de cada biblioteca.
4. **Si necesita ayuda para comprender cuál de sus aplicaciones usa ADAL**, le recomendamos que revise todos los códigos fuente de sus aplicaciones. Si procede, puede contactar con cualquier proveedor de software independiente (ISV) o con proveedores de aplicaciones. El soporte técnico de Microsoft también puede proporcionarle una lista de todas las aplicaciones ADAL que no son de Microsoft en su espacio empresarial.







