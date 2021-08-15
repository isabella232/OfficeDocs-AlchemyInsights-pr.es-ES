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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986836"
---
# <a name="issues-with-credentials"></a>Problemas con las credenciales

Plataforma de identidad de Microsoft y el flujo de credenciales de cliente de [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describe cómo programar directamente con el flujo de concesión de credenciales de cliente de OAuth 2.0.

**¿Cómo puedo administrar las credenciales de certificado o contraseña de una aplicación?**

En la CLI de Azure, puedes usar la credencial [az ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, enumerar o restablecer las credenciales de certificado o contraseña de una aplicación.

**¿Cómo pueden mis usuarios restablecer sus propias contraseñas?**

Los usuarios deben [registrarse para el restablecimiento de contraseñas de](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) autoservicio antes de poder restablecer sus contraseñas. Una vez que un usuario se haya registrado, puede seguir las instrucciones de este artículo para restablecer su contraseña: Restablecer la contraseña del trabajo [o la escuela.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**¿Cómo pueden mis usuarios cambiar sus propias contraseñas?**

Los usuarios pueden seguir los pasos de este artículo para cambiar sus contraseñas: [Cómo cambiar la contraseña](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
También pueden administrar [contraseñas de aplicaciones para la comprobación en dos pasos.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mi usuario recibe un error al cambiar o restablecer su contraseña**

Este vínculo proporcionará información sobre problemas comunes que pueden surgir cuando un usuario está intentando restablecer su contraseña: [problemas comunes y sus soluciones](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Tengo un problema al restablecer la contraseña de un usuario**

- Asegúrese de que está autorizado a restablecer las contraseñas. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

- Asegúrese de comprender los requisitos de licencias:

  - Debe tener al menos una licencia asignada en su organización:
    - **Solo usuarios en la** nube: sku Office 365 (O365) de pago o Azure AD Basic
    - **Usuarios locales o** en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Para obtener más información sobre los requisitos de licencias, consulte [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Para restablecer la contraseña de un usuario, busque el usuario en Azure AD. A continuación, en la hoja de información general para ese usuario, haga clic en el botón "Restablecer contraseña".

**El botón de restablecimiento de contraseña está gris**

No está autorizado a restablecer **las contraseñas** de este usuario. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de restablecimiento de contraseña**

No está autorizado a restablecer contraseñas. *Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.* Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de integración local en el restablecimiento de contraseñas**

- La hoja de integración local solo aparece en entornos híbridos, lo que significa que usa la escritura de escritura por contraseña para manipular las contraseñas del usuario local.

- No verá esta hoja si:

  - No está usando la reescribición de contraseñas
  - Hay un problema con la instalación/conectividad de la escritura por escritura por contraseña
  - Hay un problema con la instalación o conectividad de Azure AD Conectar
  - Para obtener más pasos de solución de problemas con la reescribición de contraseñas, consulte [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**No sé cómo restablecer la contraseña de un usuario**

1. Inicie sesión en Azure Portal como administrador adecuado.
2. Vaya a la **hoja Usuarios y grupos,** seleccione **Todos los usuarios**.
3. Seleccione un usuario de la lista.
4. Para el usuario seleccionado, seleccione **Información general** y, a continuación, en la barra de comandos, seleccione **Restablecer contraseña**.
5. Seleccione el **botón Restablecer contraseña** y siga las instrucciones que aparecen en la pantalla.
    - Solo se restablecen los restablecimientos realizados a través de la reescribición de contraseñas de soporte técnico de **Azure Portal.**

**Restablezca la contraseña de un usuario local desde el portal de Office 365 Admin o Office 365 aplicación móvil, pero el usuario aún no puede iniciar sesión**

La escritura de contraseña no se admite en este portal. Restablezca la contraseña del usuario de nuevo en Azure Portal.
