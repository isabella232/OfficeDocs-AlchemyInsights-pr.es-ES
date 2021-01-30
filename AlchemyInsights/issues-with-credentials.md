---
title: Problemas con las credenciales
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052956"
---
# <a name="issues-with-credentials"></a>Problemas con las credenciales

La plataforma de identidad de Microsoft y el flujo de credenciales de cliente de [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describen cómo programar directamente con el flujo de concesión de credenciales de cliente de OAuth 2.0.

**¿Cómo puedo administrar las credenciales de certificado o contraseña de una aplicación?**

En la CLI de Azure, puedes usar la credencial az [ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, enumerar o restablecer las credenciales de certificado o contraseña de una aplicación.

**¿Cómo restablecen mis usuarios sus contraseñas?**

Los usuarios deben [registrarse para el restablecimiento](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) de contraseña de autoservicio antes de poder restablecer sus contraseñas. Una vez que un usuario se ha registrado, puede seguir las instrucciones de este artículo para restablecer su contraseña: Restablecer la contraseña del trabajo o [la escuela.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**¿Cómo cambian mis usuarios sus contraseñas?**

Los usuarios pueden seguir los pasos de este artículo para cambiar sus contraseñas: [Cómo cambiar la contraseña.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
También pueden administrar [contraseñas de aplicaciones para la verificación en dos pasos.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mi usuario recibe un error al cambiar o restablecer su contraseña**

Este vínculo proporcionará información sobre problemas comunes que pueden surgir cuando un usuario intenta restablecer su contraseña: problemas [comunes y sus soluciones](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Tengo un problema al restablecer la contraseña de un usuario**

- Asegúrese de que está autorizado a restablecer contraseñas. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

- Asegúrese de comprender los requisitos de licencia:

  - Debe tener al menos una licencia asignada en su organización:
    - **Solo usuarios en la** nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic
    - **Usuarios locales o en** la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Para obtener más información sobre los requisitos de licencia, consulte Requisitos de licencia para el restablecimiento de contraseña de autoservicio [de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Para restablecer la contraseña de un usuario, busque el usuario en Azure AD. A continuación, en la hoja de información general para ese usuario, haga clic en el botón "restablecer contraseña".

**El botón de restablecimiento de contraseña está en gris**

No está autorizado a restablecer las **contraseñas** de este usuario. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de restablecimiento de contraseña**

No está autorizado a restablecer contraseñas. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de integración local en el restablecimiento de contraseña**

- La hoja de integración local solo aparece en entornos híbridos, lo que significa que usa la escritura de contraseña para manipular las contraseñas de los usuarios locales.

- Esta hoja no se ve si:

  - No está usando la escritura reescribición de contraseñas
  - Hay un problema con la instalación o conectividad de la escritura de contraseña
  - Hay un problema con la instalación y conectividad de Azure AD Connect
  - Para obtener más información sobre los pasos de solución de problemas con la escritura reescribición de contraseñas, vea [Solucionar problemas de](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback) escritura de contraseña

**No sé cómo restablecer la contraseña de un usuario**

1. Inicie sesión en Azure Portal como administrador adecuado.
2. Vaya a la **hoja Usuarios y grupos,** seleccione **Todos los usuarios.**
3. Seleccione un usuario de la lista.
4. Para el usuario seleccionado, seleccione **Información general** y, a continuación, en la barra de comandos, seleccione **Restablecer contraseña.**
5. Seleccione el **botón Restablecer contraseña** y siga las instrucciones de la pantalla.
    - Solo los restablecimientos realizados a través de **Azure Portal** admiten la reescribición de contraseñas.

**Restablecido la contraseña de un usuario local desde el portal de administración de Office 365 o la aplicación móvil de Office 365, pero el usuario aún no puede iniciar sesión**

La escritura escritura en contraseña no se admite en este portal. Restablezca la contraseña del usuario de nuevo en Azure Portal.
