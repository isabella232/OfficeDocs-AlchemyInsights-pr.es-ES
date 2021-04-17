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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820303"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="fe75b-102">Acceso a claves de recuperación de Bitlocker</span><span class="sxs-lookup"><span data-stu-id="fe75b-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="fe75b-103">Al configurar la configuración de Bitlocker Intune Endpoint Protection Policy, es posible definir si la información de recuperación de Bitlocker debe almacenarse en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fe75b-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="fe75b-104">Si esa configuración está configurada, los datos de recuperación almacenados deben ser visibles para un administrador de Intune como parte de los datos de registro de dispositivos en la hoja Dispositivos intunees de dos maneras:</span><span class="sxs-lookup"><span data-stu-id="fe75b-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="fe75b-105">Dispositivos: dispositivos de Azure AD -> "Dispositivo" O dispositivos -> Todos los dispositivos -> "Dispositivo" -> claves de recuperación</span><span class="sxs-lookup"><span data-stu-id="fe75b-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="fe75b-106">Como alternativa, si hay acceso administrativo al propio dispositivo, la clave de recuperación (Contraseña) se puede ver ejecutando el siguiente comando desde un símbolo del sistema con privilegios elevados:</span><span class="sxs-lookup"><span data-stu-id="fe75b-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="fe75b-107">Si el dispositivo se cifraba antes de la inscripción en Intune, es posible que la clave de recuperación se haya asociado con la "cuenta de Microsoft" (MSA) usada para iniciar sesión en el dispositivo durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="fe75b-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="fe75b-108">En ese caso, el acceso y la sesión con esa MSA deben mostrar los dispositivos para los que se almacenaron  https://onedrive.live.com/recoverykey las claves de recuperación.</span><span class="sxs-lookup"><span data-stu-id="fe75b-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="fe75b-109">Si el dispositivo se cifra como resultado de la configuración a través de una directiva de grupo basada en dominio, la información de recuperación puede almacenarse en Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="fe75b-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="fe75b-110">Si has configurado la directiva de protección de puntos de conexión para almacenar la clave de recuperación en Azure Active Directory pero no se ha cargado la clave de un dispositivo específico, puedes desencadenar la carga girando la clave de recuperación para ese dispositivo desde la consola de MEM.</span><span class="sxs-lookup"><span data-stu-id="fe75b-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="fe75b-111">Para obtener más información, [consulta Girar claves de recuperación de BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="fe75b-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

