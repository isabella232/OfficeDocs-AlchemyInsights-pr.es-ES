---
title: La reescribición de contraseñas no funciona
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324940"
---
# <a name="password-writeback-is-not-working"></a>La reescribición de contraseñas no funciona

**Tengo problemas para configurar la reescribición de contraseñas**

- La reescribición de contraseñas es una característica premium.
- Asegúrese de comprender los requisitos de licencias:
  - Debe tener al menos una licencia asignada en su organización
  - **Solo usuarios en la** nube: sku Office 365 (O365) de pago o Azure AD Basic
  - **Usuarios locales o** en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Para obtener más información sobre los requisitos de licencias, consulte [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Tiene al menos una cuenta de administrador y una cuenta de usuario de prueba con una de la licencia adecuada.
- Debe conectar Azure AD Conectar al controlador de dominio principal Emulator para que la escritura de contraseña funcione. Puede configurar Azure AD Conectar usar un controlador de dominio  principal haciendo clic con el botón secundario en las propiedades del conector de sincronización de Active Directory y, a continuación, **seleccionando configurar particiones de directorio**. A partir de ahí, busque la sección **configuración** de conexión del controlador de dominio y active la casilla titulada **solo usar controladores de dominio preferidos.**
    **Nota**:Si el CONTROLADOR de dominio preferido no es un emulador de PDC, Azure AD Conectar se pondrá en contacto con la PDC para la reescribición de contraseñas.
- El restablecimiento de contraseña se ha configurado y habilitado en el espacio empresarial. Para obtener más información, vea [Permitir que los usuarios restablezcan sus contraseñas de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Asegúrese de que la cuenta de administrador que se usa para habilitar la reescribición de contraseñas sea una cuenta de administrador en la nube (creada en Azure AD no en AD local)
- Tiene una implementación local de AD única o de varios bosques que ejecuta Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con los service pack más recientes instalados
- Tiene instalada la herramienta Conectar azure AD y ha preparado el entorno de AD para la sincronización en la nube. Antes de probar la reescribición de contraseñas, asegúrate de completar primero una importación completa y una sincronización completa de AD y Azure AD en Azure AD Conectar.
- Para obtener más información, vea cómo realizar una sincronización completa e [importación completa en Azure AD Conectar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Tengo un problema con la conectividad de reescribición de contraseñas**

1. Descargar y habilitar la versión más reciente de [Azure AD Conectar](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuración del firewall: la herramienta Conectar azure AD (1.1.443 y posteriores) necesitará acceso **HTTPS** saliente a:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permitir que las conexiones inactivas persistan durante al menos 2-3 minutos

**Todavía tengo problemas con la reescribición de contraseñas**

- Si aún tiene dificultades, intente deshabilitar y volver a habilitar el servicio de escritura difis de contraseña en la herramienta de escritura Conectar Azure AD
- Para obtener más información, vea cómo deshabilitar y volver a habilitar la escritura [dise? de contraseña](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
