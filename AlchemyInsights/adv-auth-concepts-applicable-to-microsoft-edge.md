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
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934382"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Conceptos de autenticación avanzada aplicables a Microsoft Edge

Estos son los conceptos de autenticación avanzada que se aplican a Microsoft Edge:

**Autenticación proactiva**

Al habilitar la directiva [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge intentará autenticar de forma proactiva a los usuarios que han iniciado sesión a través de servicios Microsoft. A intervalos regulares, usará un servicio en línea para buscar un manifiesto actualizado que contenga la configuración que rige la autenticación proactiva.

Ventajas: la autenticación proactiva permite la autenticación en servicios clave, como la Office nueva pestaña. Además, si Bing se usa como motor de búsqueda, la autenticación proactiva mejora el rendimiento de la barra de direcciones y ayuda a generar resultados de búsqueda personalizados a las necesidades de su empresa.

**Windows Hello CredUI para autenticación NTLM**

Si el inicio de sesión único (SSO) no está disponible cuando un sitio web intenta iniciar sesión en el usuario mediante el mecanismo NTLM o Negotiate, esta característica permitirá al usuario compartir las credenciales del sistema operativo con el sitio web y satisfacer el desafío de autenticación mediante Windows Hello Cred UI. Este flujo de inicio de sesión solo aparecerá en Windows 10 y solo para los usuarios que no obtienen SSO durante un NTLM o un desafío Negotiate.

**Usar contraseñas guardadas para iniciar sesión automáticamente**

Los usuarios que guardan contraseñas en Microsoft Edge pueden habilitar el inicio de sesión automático en sitios web donde han guardado credenciales. Los usuarios pueden activar o desactivar esta característica en edge://settings/passwords y puede configurarla en las directivas del [administrador de](https://go.microsoft.com/fwlink/?linkid=2134622) contraseñas.
