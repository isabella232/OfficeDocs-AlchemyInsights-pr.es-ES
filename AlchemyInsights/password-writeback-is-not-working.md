---
title: La escritura reescribición de contraseñas no funciona
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232785"
---
# <a name="password-writeback-is-not-working"></a>La escritura por escritura no funciona

**Tengo problemas para configurar la escritura difisura de contraseñas**

- La escritura reescribición de contraseñas es una característica premium.
- Asegúrese de que comprende los requisitos de licencia:
  - Debe tener al menos una licencia asignada en su organización
  - **Solo usuarios en la** nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic
  - **Usuarios locales o** en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
    - Para obtener más información sobre los requisitos de licencia, consulte [Requisitos de licencias](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) para el restablecimiento de contraseña de autoservicio de Azure AD
- Tiene al menos una cuenta de administrador y una cuenta de usuario de prueba con una de las licencias adecuadas.
- Debe conectar Azure AD Connect al emulador del controlador de dominio principal para que funcione la escritura reescribición de contraseñas. Puede configurar Azure AD Connect para usar un controlador  de dominio principal haciendo clic con el botón secundario en las propiedades del conector de sincronización de Active Directory y, a continuación, **seleccionando configurar particiones de directorio.** Desde allí, busque la sección de configuración **de** conexión del controlador de dominio y active la casilla titulada **solo usar controladores de dominio preferidos.**
  > [!NOTE]
  > Si el DC preferido no es un emulador de PDC, Azure AD Connect seguirá llegando a la PDC para la escritura en contraseña.
- El restablecimiento de contraseña se ha configurado y habilitado en el espacio empresarial. Para obtener más información, vea [Habilitar a los usuarios para restablecer sus contraseñas de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Asegúrese de que la cuenta de administrador que se usa para habilitar la reescribición de contraseñas sea una cuenta de administrador en la nube (creada en Azure AD no en AD local)
- Tiene una implementación local de AD de bosque único o de varios bosques que ejecuta Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con los Service Pack más recientes instalados
- Tiene instalada la herramienta Azure AD Connect y ha preparado su entorno de AD para la sincronización con la nube. Antes de probar la escritura reescribición de contraseñas, asegúrate de completar primero una importación completa y una sincronización completa de AD y Azure AD en Azure AD Connect.
- Para obtener más información, vea cómo realizar una sincronización completa e [importación completa en Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**I'm having a problem with password writeback connectivity**

1. Descargar y habilitar la última versión de [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuración del firewall: la herramienta Azure AD Connect (1.1.443 y posteriores) necesitará acceso **HTTPS** saliente para:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permitir que las conexiones inactivas persistan durante al menos 2 o 3 minutos

**I'm still having problems with password writeback**

- Si sigue teniendo dificultades, intente deshabilitar y volver a habilitar el servicio de escritura difis para contraseñas en la herramienta Azure AD Connect
- Para obtener más información, vea cómo deshabilitar y volver a habilitar la escritura [difi ón de contraseña](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
