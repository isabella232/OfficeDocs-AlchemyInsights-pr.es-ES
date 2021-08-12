---
title: 646 Cómo configurar AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963660"
---
# <a name="configure-sync-features"></a>Configurar características de sincronización

Azure AD Conectar incluye varias características que están habilitadas de forma predeterminada o que puede habilitar más adelante. Algunas características requieren configuración adicional en entornos específicos.

- [Los](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) límites de filtrado de los objetos se sincronizan con Azure AD. De forma predeterminada, se sincronizan todos los usuarios, contactos, grupos y Windows 10 cuentas de equipo. Puede incluir o excluir objetos basados en dominios, US u otros atributos.

- [La sincronización de hash de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) contraseña sincroniza el hash de contraseña de Active Directory local a Azure AD. Esto permite la administración de contraseñas en una ubicación, pero el uso de la misma contraseña en entornos locales y en la nube. Dado que Active Directory es el origen autoritativo, puede usar sus propias directivas de contraseña.

- [El restablecimiento de contraseñas de autoservicio (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite a los usuarios restablecer sus propias contraseñas en la nube mientras siguen aplicando la directiva de contraseña local.

- [La reescribición](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) de dispositivos permite que los dispositivos registrados en Azure AD se vuelvan a escribir en Active Directory local para que se puedan usar para el acceso condicional.

- [Evitar eliminaciones accidentales](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) está habilitada de forma predeterminada para ayudar a evitar demasiadas eliminaciones simultáneas de objetos (más de 500 objetos por sincronización). Puede cambiar esta configuración para satisfacer las necesidades de su organización.

- [La actualización](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) automática está habilitada de forma predeterminada para instalaciones express y ayuda a garantizar que la versión de Azure AD Conectar esté siempre actualizada.
