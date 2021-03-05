---
title: Solucionar problemas de SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428832"
---
# <a name="troubleshoot-sspr"></a>Solucionar problemas de SSPR

**Tengo problemas para configurar el restablecimiento de contraseñas**

- Si es administrador y está buscando cómo habilitar el restablecimiento de contraseñas de autoservicio, vea [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization. También es posible que desee revisar los [requisitos de licencia](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Debe tener al menos una licencia asignada en su organización.
    - **Solo usuarios en la** nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic
    - **Usuarios locales o** en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)
- Para obtener preguntas adicionales sobre el restablecimiento de contraseñas de autoservicio, revise [nuestras preguntas más frecuentes](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Obtención de un mensaje de error**

Revise este artículo para encontrar errores comunes y sus soluciones: [Solucionar problemas de restablecimiento de contraseñas de autoservicio](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tengo un problema con mi directiva de restablecimiento de contraseña**

- Si la directiva de restablecimiento de contraseña no se comporta como se esperaba o si tiene preguntas acerca de las directivas de restablecimiento de contraseña, consulte este artículo: Directivas de contraseña [y restricciones](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)en Azure Active Directory .
- Las directivas de restablecimiento de contraseña no se aplican a los administradores. Microsoft aplica una directiva de restablecimiento de contraseña de dos puertas predeterminada para cualquier rol de administrador de Azure. Asegúrese de que está probando con un usuario que no es administrador. Para obtener más información sobre la directiva de restablecimiento de administrador, vea este artículo: [Diferencias de directiva de restablecimiento de administrador.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**No quiero que mis usuarios registren información de seguridad adicional para el restablecimiento de contraseñas**

Puede rellenar previamente los datos (atributos de correo electrónico y teléfono) para los usuarios mediante una API, PowerShell o Azure AD Connect. Para obtener información sobre cómo leer:

- [Implementar el restablecimiento de contraseña sin necesidad de que los usuarios se registren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Qué datos usa el restablecimiento de contraseña](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Deseo que mis usuarios registren su información de seguridad adicional para el restablecimiento de contraseñas**

1. Pide a los usuarios que registren su información de seguridad para el restablecimiento de contraseñas de autoservicio al dirigirlos a [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Después de rellenar los datos para el usuario (por el usuario o por el administrador), dirija al usuario [a aka.ms/sspr](https://passwordreset.microsoftonline.com/) para que los usuarios puedan tener la capacidad de restablecer sus propias contraseñas.
1. Si los usuarios siguen experimentando problemas, lo más probable es que sean usuarios **federados** o con **hash de contraseña sincronizados.** Esto significa que es probable que haya un problema con el servicio de reescribición de contraseñas.