---
title: Habilitar autenticación SMTP y solución de problemas
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
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321770"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Habilitar autenticación SMTP y solución de problemas

Si desea habilitar la autenticación SMTP para un buzón o recibe un error "Cliente no autenticado", "Autenticación incorrecta" o "SmtpClientAuthentication" con el código 5.7.57, 5.7.3 o 5.7.139 al intentar retransmitir correo electrónico mediante la autenticación de un dispositivo o aplicación con Microsoft 365, realice estas tres acciones para resolver el problema:

1. Deshabilite los [Valores predeterminados de seguridad de Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). Para ello, establezca **Habilitar los valores predeterminados de seguridad** en **No**.

    a. Inicie sesión en Azure Portal como administrador de seguridad, administrador de acceso condicional o administrador global.<BR/>
    b. Vaya a Azure Active Directory >  **Propiedades**.<BR/>
    c. Seleccione **Administrar los valores predeterminados de seguridad**.<BR/>
    d. Establezca **Habilitar los valores predeterminados de seguridad** en **No**.<BR/>
    e. Seleccione **Guardar**.

2. Marque [Habilitar el envío de SMTP de cliente](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) en el buzón con licencia.

    a. En el Centro de administración de Microsoft 365, vaya a **Usuarios activos** y seleccione el usuario.<BR/>
    b. Vaya a la pestaña Correo y, en **Aplicaciones de correo electrónico**, seleccione **Administrar aplicaciones de correo electrónico**.<BR/>
    d. Asegúrese de que **SMTP autenticado** esté activado (habilitado).<BR/>
    e. Seleccione **Guardar cambios**.<BR/>

3. Marque [Deshabilitar la autenticación multifactor (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) en el buzón con licencia.

    a. Vaya al Centro de administración de Microsoft 365 y, en el menú de navegación izquierdo, seleccione **Usuarios** > **Usuarios activos**.<BR/>
    b. Seleccione **Autenticación multifactor**.<BR/>
    c. Seleccione el usuario y deshabilite **Autenticación multifactor**.<BR/>
