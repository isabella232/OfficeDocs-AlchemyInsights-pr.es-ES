---
title: 451 4.7.0 Error de servidor temporal. Inténtelo de nuevo más tarde. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 16e16f087c2b13a9ad5fec7223b4f3395e42646e
ms.sourcegitcommit: 380ee556007d2be389b1a99795bca04bc1f9f60f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/27/2021
ms.locfileid: "53604940"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Error de servidor temporal. Inténtelo de nuevo más tarde. PRX4

Es posible que tenga un problema al enviar correo electrónico a través de Smarthost "smtp.office365.com" mediante el método de envío de cliente SMTP y recibir el error: "Error de servidor temporal 451 4.7.0. Inténtelo de nuevo más tarde. PRX4 es principalmente temporal". 

Asegúrese de que no está usando un buzón compartido para el envío de cliente SMTP, ya que el método de envío de cliente SMTP requiere un buzón con licencia para enviar correo. Sin embargo, si no usa un buzón compartido y el problema persiste, compruebe lo siguiente:

1. Habilite el envío SMTP de cliente en el buzón con licencia que se usa ejecutando este comando de PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    O

    1. Vaya a la Centro de administración de Microsoft 365 > **Usuarios activos** y seleccione el usuario.
    1. Vaya a la pestaña Correo > **aplicaciones de** correo > seleccione Administrar aplicaciones de **correo electrónico.** 
    1. Asegúrese de que **la configuración SMTP autenticada** está activada (habilitada).
    1. Seleccione **Guardar cambios**.
    
    Para habilitar la autenticación SMTP para toda una organización, ejecute este comando:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Nota:** Por motivos de seguridad, se recomienda habilitar la autenticación SMTP solo para el buzón que se está utilizando. La configuración de nivel de usuario invalida la configuración de nivel de organización.

2. Deshabilite los valores predeterminados de Azure Security al alternar Habilitar valores predeterminados **de seguridad** en **No:**

    1. Inicie sesión en Azure Portal como administrador de seguridad, administrador de acceso condicional o administrador global.
    1. Vaya a Azure Active Directory >**  Propiedades** y seleccione **Administrar valores predeterminados de seguridad**.
    1. Establezca la **opción Habilitar valores predeterminados de seguridad** en **No**.
    1. Seleccione **Guardar**.

3. Deshabilite la autenticación multifactor (MFA) en el buzón con licencia que se está utilizando.

    1. Vaya a la Centro de administración de Microsoft 365 y, en el menú de navegación izquierdo, elija **Usuarios**  >  **usuarios activos.**
    1. En la página **Usuarios activos**, elija **Autenticación multifactor**.
    1. Seleccione el usuario y deshabilite **la autenticación multifactor**.

