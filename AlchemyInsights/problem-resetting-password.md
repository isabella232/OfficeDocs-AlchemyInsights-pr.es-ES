---
title: Problema al restablecer la contraseña
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: fe3a13acb0ba5c8872d7c0bb8c3961d83f7d3526
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568696"
---
# <a name="problems-resetting-password"></a>Problemas para restablecer la contraseña

Estos son algunos de los problemas que puede tener que enfrentar al restablecer la contraseña y las posibles soluciones:

**Tengo un problema con el restablecimiento de contraseña no cubierto en las otras categorías**

-Asegúrese de que está autorizado a restablecer las contraseñas. Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario. Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.
- Asegúrese de comprender los requisitos de licencia:
    - Debe tener al menos una licencia asignada en su organización
        - Solo usuarios en la nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic
        - Usuarios locales o en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
        - Para obtener más información acerca de los requisitos de licencias, consulte el artículo Requisitos de licencias para el restablecimiento de contraseñas de autoservicio [de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tengo problemas para probar la directiva de restablecimiento de contraseña que he establecido**

- Las directivas aplicadas recientemente pueden tardar varios minutos en replicarse en todos los centros de datos y puntos finales. La distancia física desde el centro de datos también afectará a la rapidez con la que se aplican los cambios.
- Pruebe con un usuario final, no con un administrador y piloto con un pequeño conjunto de usuarios. Las directivas configuradas en Azure Portal SOLO se aplican a los usuarios finales, no a los administradores. Microsoft aplica una directiva de restablecimiento de contraseña de dos puertas predeterminada para cualquier rol de administrador de Azure (ejemplo: administrador global, administrador del departamento de soporte técnico, administrador de contraseñas, etc.)
    - Obtenga más información sobre [las directivas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Quiero implementar el restablecimiento de contraseña, pero no quiero que mis usuarios registren información de seguridad adicional**

Rellena previamente los datos de los usuarios para que no tengan que hacerlo. - Como administrador, puede establecer propiedades de teléfono y correo electrónico para los usuarios antes de implementar el restablecimiento de contraseña en su organización. Puede hacerlo con una API, PowerShell o Azure AD Connect. Más información aquí:
- [Implementar el restablecimiento de contraseña sin necesidad de que los usuarios se registren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Qué datos usa el restablecimiento de contraseña](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**El botón de restablecimiento de contraseña está gris**

No está autorizado a restablecer las contraseñas de este usuario. Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario. Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de restablecimiento de contraseña**

No está autorizado a restablecer contraseñas. Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario. Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.

**No veo la hoja de integración local en el restablecimiento de contraseñas**

- La hoja de integración local solo aparece en entornos híbridos, lo que significa que usa la escritura de escritura por contraseña para manipular las contraseñas del usuario local.
- No verá esta hoja si:
    - No está usando la reescribición de contraseñas
    - Hay un problema con la instalación/conectividad de la escritura por escritura por contraseña
    - Hay un problema con la instalación/conectividad de Azure AD Connect
    - Para obtener más pasos de solución de problemas con la escritura reescribición de contraseñas, vea la sección Solucionar problemas [de escritura contra escritura de contraseñas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**No sé cómo restablecer la contraseña de un usuario**

1. Inicie sesión en Azure Portal como administrador adecuado.
1. Vaya a la hoja Usuarios y grupos, seleccione **Todos los usuarios**.
1. Seleccione un usuario de la lista.
1. Para el usuario seleccionado, seleccione **Información general** y, a continuación, en la barra de comandos, haga clic en **Restablecer contraseña.**
1. Siga las instrucciones de la pantalla.
    - Solo se restablecen los restablecimientos realizados a través de la reescribición de contraseñas de soporte técnico de Azure Portal.

**Restablezca la contraseña de un usuario local desde el portal de administración de Office 365 o la aplicación móvil de Office 365, pero el usuario aún no puede iniciar sesión**

La escritura de contraseña no se admite en este portal. Restablecer la contraseña del usuario de nuevo en Azure Portal: portal.azure.com

