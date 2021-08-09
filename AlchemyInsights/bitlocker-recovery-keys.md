---
title: Claves de recuperación de Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060081"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Acceso a claves de recuperación de Bitlocker

Al configurar la directiva de configuración de Bitlocker Endpoint Protection Intune, es posible definir si la información de recuperación de Bitlocker debe almacenarse en Azure Active Directory.

Si esa configuración está configurada, los datos de recuperación almacenados deben ser visibles para un administrador de Intune como parte de los datos de registro de dispositivos en la hoja Dispositivos intunees de dos maneras:

Dispositivos: dispositivos de Azure AD -> "Dispositivo" O dispositivos -> Todos los dispositivos -> "Dispositivo" -> claves de recuperación

Como alternativa, si hay acceso administrativo al propio dispositivo, la clave de recuperación (Contraseña) se puede ver ejecutando el siguiente comando desde un símbolo del sistema con privilegios elevados:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Si el dispositivo se cifraba antes de la inscripción en Intune, es posible que la clave de recuperación se haya asociado con la "cuenta de Microsoft" (MSA) usada para iniciar sesión en el dispositivo durante el proceso de OOBE. En ese caso, el acceso y la sesión con esa MSA deben mostrar los dispositivos para los que se almacenaron  https://onedrive.live.com/recoverykey las claves de recuperación.
 
Si el dispositivo se cifra como resultado de la configuración a través de una directiva de grupo basada en dominio, la información de recuperación puede almacenarse en Active Directory local.

Si has configurado la directiva de protección de puntos de conexión para almacenar la clave de recuperación en Azure Active Directory pero no se ha cargado la clave de un dispositivo específico, puedes desencadenar la carga girando la clave de recuperación de ese dispositivo desde la consola de MEM. Para obtener más información, [consulta Girar claves de recuperación de BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

