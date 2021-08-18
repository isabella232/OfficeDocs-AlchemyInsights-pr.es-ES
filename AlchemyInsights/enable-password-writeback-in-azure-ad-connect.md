---
title: Habilitar la escritura diferida en Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325404"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Habilitar la escritura diferida en Azure AD Connect

Para habilitar el restablecimiento de contraseña de autoservicio, habilite primero la opción de reescritura en Azure AD Connect. Desde el servidor de Azure AD Connect, siga los pasos que se indican a continuación:

1. Inicie sesión en el servidor de Azure AD Connect e inicie el **Asistente para la configuración de Azure AD Connect**.
2. En la página de **Bienvenida**, haga clic en **Configurar**.
3. En la página **Tareas adicionales**, haga clic en **Personalizar las opciones de sincronización** y, a continuación, haga clic en **Siguiente**.
4. En la página Conectarse a Azure AD, escriba una credencial de administrador global para su inquilino de Azure y haga clic en siguiente.
5. En las páginas **Conectar directorios** y **Filtrado de dominios y unidades organizativas**, haga clic en **Siguiente**.
6. En la página **Características opcionales**, seleccione la casilla junto a **Contraseña con escritura diferida** y haga clic en **Siguiente**.
7. En la página **Preparado para configurar**, haga clic en **Configurar** y espere a que finalice el proceso.
8. Cuando vea finalizar la configuración, haga clic en **Salir**.

Con la escritura a contraseña diferida en Azure AD Connect, ahora configure Azure AD SSPR para la reescritura.  Para habilitar la escritura diferida en SSPR, siga los pasos que se indican a continuación:

1. Inicie sesión en Microsoft Azure Portal con una cuenta de administrador global.
2. Busque y seleccione **Azure Active Directory**, haga clic en **Restablecer contraseña** y, a continuación, elija **Integración local**.
3. Establecer la opción de **¿Reescribir contraseñas en el directorio local?** en **Sí**.
4. Establecer la opción de **¿Permitir que los usuarios puedan desbloquear cuentas sin restablecer su contraseña?** a **Sí**.
5. Cuando haya terminado, haga clic en **Aceptar**.

Para obtener más información, consulte [Habilitar la reescritura diferida de la contraseña de autoservicio de Azure Active Directory en un entorno local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

**Nota**: cuando un administrador restablece la contraseña de un usuario en Azure Portal, si ese usuario es federado o se sincroniza con hash de contraseña, la contraseña se vuelve a escribir en local. Esta funcionalidad necesita de una licencia Azure Premium (P1 o P2) y que actualmente no está respaldada en el portal de Administrador de Office.
