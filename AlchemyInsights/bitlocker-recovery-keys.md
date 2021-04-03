---
title: Claves de recuperación de Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505085"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Acceso a claves de recuperación de Bitlocker

Al configurar la configuración de Bitlocker Intune Endpoint Protection Policy, es posible definir si la información de recuperación de Bitlocker debe almacenarse en Azure Active Directory.

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

Si has configurado la directiva de protección de puntos de conexión para almacenar la clave de recuperación en Azure Active Directory pero no se ha cargado la clave de un dispositivo específico, puedes desencadenar la carga girando la clave de recuperación para ese dispositivo desde la consola de MEM. Para obtener más información, [consulta Girar claves de recuperación de BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

