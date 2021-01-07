---
title: Dataprotection-BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768834"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="18ce2-102">Habilitación del cifrado de BitLocker con Intune</span><span class="sxs-lookup"><span data-stu-id="18ce2-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="18ce2-103">La Directiva de la protección de extremos de Intune se puede usar para configurar las opciones de cifrado de BitLocker para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="18ce2-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="18ce2-104">Para obtener más información, consulte [configuración de Windows 10 (y versiones posteriores) para proteger los dispositivos con Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="18ce2-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="18ce2-105">Debe tener en cuenta que muchos dispositivos nuevos que ejecutan Windows 10 admiten el cifrado de BitLocker automático, que se desencadena sin la aplicación de la Directiva de MDM.</span><span class="sxs-lookup"><span data-stu-id="18ce2-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="18ce2-106">Esto puede afectar a la aplicación de la Directiva si se configuran opciones no predeterminadas.</span><span class="sxs-lookup"><span data-stu-id="18ce2-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="18ce2-107">Consulte las siguientes preguntas frecuentes para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="18ce2-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="18ce2-108">Para obtener información sobre cómo solucionar problemas de BitLocker, vea [solucionar problemas de las directivas de BitLocker en Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="18ce2-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="18ce2-109">**Preguntas frecuentes**</span><span class="sxs-lookup"><span data-stu-id="18ce2-109">**FAQ**</span></span>

<span data-ttu-id="18ce2-110">P: ¿Qué ediciones de Windows admiten el cifrado de dispositivos con la Directiva de Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="18ce2-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="18ce2-111">A: la configuración de la Directiva de la protección de extremos de Intune se implementa con el [CSP de BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="18ce2-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="18ce2-112">No todas las ediciones o compilaciones de Windows admiten el CSP de BitLocker.</span><span class="sxs-lookup"><span data-stu-id="18ce2-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="18ce2-113">P: ¿cómo se puede habilitar BitLocker en dispositivos sin que sea necesaria la interacción del usuario final?</span><span class="sxs-lookup"><span data-stu-id="18ce2-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="18ce2-114">A: siempre que se cumplan los requisitos previos necesarios, es posible habilitar el "cifrado silencioso" de BitLocker a través de Intune.</span><span class="sxs-lookup"><span data-stu-id="18ce2-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="18ce2-115">Vea los detalles de la configuración de directiva de ejemplo y los requisitos de dispositivo para habilitar el cifrado silencioso en el siguiente documento: [Habilitar el cifrado de BitLocker en modo silencioso](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="18ce2-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="18ce2-116">P: Si ya se ha cifrado un dispositivo con BitLocker mediante la configuración predeterminada del sistema operativo para el método de cifrado y la seguridad de cifrado (XTS-AES-128), se aplicará una directiva con una configuración diferente para activar de nuevo el cifrado de la unidad con la nueva configuración.</span><span class="sxs-lookup"><span data-stu-id="18ce2-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="18ce2-117">R: No.</span><span class="sxs-lookup"><span data-stu-id="18ce2-117">A: No.</span></span> <span data-ttu-id="18ce2-118">Para aplicar la nueva configuración de cifrado, primero debe descifrarse la unidad.</span><span class="sxs-lookup"><span data-stu-id="18ce2-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="18ce2-119">**Nota:** Para los dispositivos que se inscriben con AutoPilot, el cifrado automático que se produciría durante la OOBE no se desencadena hasta que se evalúe la Directiva de Intune, lo que permite usar la configuración basada en directivas en lugar de los valores predeterminados del sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="18ce2-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="18ce2-120">P: Si un dispositivo está cifrado como resultado de la aplicación de la Directiva de Intune, ¿se descifrará cuando se quite la Directiva?</span><span class="sxs-lookup"><span data-stu-id="18ce2-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="18ce2-121">A: la eliminación de la Directiva relacionada con el cifrado no produce el descifrado de las unidades configuradas.</span><span class="sxs-lookup"><span data-stu-id="18ce2-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="18ce2-122">P: ¿por qué la Directiva de cumplimiento de Intune muestra que el dispositivo no tiene BitLocker habilitado, aunque es?</span><span class="sxs-lookup"><span data-stu-id="18ce2-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="18ce2-123">A: el valor "BitLocker Enabled" de la Directiva de cumplimiento de Intune usa el cliente de atestación de estado del dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="18ce2-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="18ce2-124">Este cliente solo mide el estado del dispositivo durante el arranque.</span><span class="sxs-lookup"><span data-stu-id="18ce2-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="18ce2-125">Por lo tanto, si un dispositivo no se ha reiniciado desde que se completó el cifrado de BitLocker, el servicio de cliente de DHA no informará de BitLocker como activo.</span><span class="sxs-lookup"><span data-stu-id="18ce2-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 