---
title: Claves de recuperación de BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685903"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="c63cd-102">Obtener acceso a las claves de recuperación de BitLocker</span><span class="sxs-lookup"><span data-stu-id="c63cd-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="c63cd-103">Al configurar la Directiva de la protección de extremos de Intune de configuración de BitLocker, es posible definir si la información de recuperación de BitLocker debe almacenarse en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c63cd-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="c63cd-104">Si esta configuración está configurada, los datos de recuperación almacenados deben estar visibles para un administrador de Intune como parte de los datos de registro de dispositivo en la hoja dispositivos de Intune de dos maneras:</span><span class="sxs-lookup"><span data-stu-id="c63cd-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="c63cd-105">Dispositivos: dispositivos de Azure AD-> "dispositivo" o dispositivos-> todos los dispositivos-> "dispositivo"-> claves de recuperación</span><span class="sxs-lookup"><span data-stu-id="c63cd-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="c63cd-106">Como alternativa, si hay acceso administrativo al propio dispositivo, se puede ver la clave de recuperación (contraseña) mediante la ejecución del siguiente comando desde un símbolo del sistema con privilegios elevados:</span><span class="sxs-lookup"><span data-stu-id="c63cd-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="c63cd-107">Si el dispositivo se cifró antes de la inscripción en Intune, es posible que la clave de recuperación se haya asociado con la "cuenta Microsoft" (MSA) que se usó para iniciar sesión en el dispositivo durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="c63cd-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="c63cd-108">Si este es el caso, el acceso  https://onedrive.live.com/recoverykey e inicio de sesión con ese MSA debería mostrar los dispositivos para los que se almacenaron claves de recuperación.</span><span class="sxs-lookup"><span data-stu-id="c63cd-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="c63cd-109">Si el dispositivo se cifró como resultado de la configuración mediante una directiva de grupo basada en dominio, la información de recuperación puede almacenarse en Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="c63cd-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

