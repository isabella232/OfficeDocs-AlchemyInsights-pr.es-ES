---
title: Conceptos de autenticación avanzada aplicables a Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571893"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceptos de autenticación avanzada aplicables a Microsoft Edge

A continuación se muestran los conceptos de autenticación avanzada aplicables a Microsoft Edge:

**Autenticación proactiva**

Al habilitar la directiva [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge intentará autenticar de forma proactiva los usuarios que han iniciado sesión a través de los servicios de Microsoft. A intervalos regulares, usará un servicio en línea para comprobar si hay un manifiesto actualizado que contenga la configuración que rige la autenticación proactiva.

Ventajas: la autenticación proactiva permite la autenticación a los servicios clave, como la página de la nueva pestaña de Office. Además, si se usa Bing como motor de búsqueda, la autenticación proactiva mejora el rendimiento de la barra de direcciones y ayuda a generar resultados de búsqueda personalizados para las necesidades de su empresa.

**Windows Hello CredUI para la autenticación NTLM**

Si el inicio de sesión único (SSO) no está disponible cuando un sitio web intenta iniciar sesión en el usuario mediante el mecanismo NTLM o Negotiate, esta característica permitirá al usuario compartir las credenciales del sistema operativo con el sitio web y cumplir el desafío de autenticación mediante la interfaz de usuario CRED de Windows Hello. Este flujo de inicio de sesión solo aparecerá en Windows 10 y solo para los usuarios que no reciban SSO durante un desafío de NTLM o de negociación.

**Usar contraseñas guardadas para iniciar sesión automáticamente**

Los usuarios que guardan contraseñas en Microsoft Edge pueden habilitar el inicio de sesión automático en los sitios web donde tienen credenciales guardadas. Los usuarios pueden activar o desactivar esta característica en edge://settings/passwords, y puede configurarla en las directivas del [Administrador de contraseñas](https://go.microsoft.com/fwlink/?linkid=2134622) .
