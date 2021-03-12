---
title: Solucionar problemas con la inscripción de dispositivos Android en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709015"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="98b33-102">Solucionar problemas con la inscripción de dispositivos Android en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="98b33-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="98b33-103">Revise los recursos que se enumeran a continuación para resolver el problema ahora.</span><span class="sxs-lookup"><span data-stu-id="98b33-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="98b33-104">Algunos problemas comunes y pasos de resolución:</span><span class="sxs-lookup"><span data-stu-id="98b33-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="98b33-105">**Error de dispositivo no cifrado en el Portal de empresa:** Las versiones más recientes de Android, especialmente a partir de v7.0, requieren un código de acceso de inicio para asegurarse de que el dispositivo está totalmente cifrado.</span><span class="sxs-lookup"><span data-stu-id="98b33-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="98b33-106">Las soluciones comunes son habilitar un pin de inicio o cifrar completamente el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98b33-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="98b33-107">Revise [este documento para](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) obtener más información.</span><span class="sxs-lookup"><span data-stu-id="98b33-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="98b33-108">Los dispositivos no pueden realizar la protección con el servicio de Intune o **mostrarse como "Incorrecto" en la consola de administración de Intune:** Es posible que algunos dispositivos Samsung 4.4 y 5.5 no entren en el servicio.</span><span class="sxs-lookup"><span data-stu-id="98b33-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="98b33-109">Hay 3 soluciones posibles para este problema:</span><span class="sxs-lookup"><span data-stu-id="98b33-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="98b33-110">Abra manualmente la aplicación Portal de empresa de Intune, que iniciará automáticamente una sincronización de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="98b33-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="98b33-111">Actualiza el dispositivo a Android 6.0 o posterior.</span><span class="sxs-lookup"><span data-stu-id="98b33-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="98b33-112">Deshabilita a Samsung Smart Manager para que no administre el Portal de empresa de Intune.</span><span class="sxs-lookup"><span data-stu-id="98b33-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="98b33-113">Revise [este documento para](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) obtener más detalles sobre estos problemas y resoluciones.</span><span class="sxs-lookup"><span data-stu-id="98b33-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="98b33-114">**Tipo de licencia de** usuario Error no válido o Nombre de usuario No **reconocido:** se debe asignar una licencia de Intune o EMS al usuario.</span><span class="sxs-lookup"><span data-stu-id="98b33-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="98b33-115">Revise estos documentos para asignar una licencia a través de: Centro de administración de Office o Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="98b33-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="98b33-116">Recursos adicionales para ayudar a resolver el problema:</span><span class="sxs-lookup"><span data-stu-id="98b33-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="98b33-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción.</span><span class="sxs-lookup"><span data-stu-id="98b33-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="98b33-118">Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles.</span><span class="sxs-lookup"><span data-stu-id="98b33-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="98b33-119">Revise [este documento para](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) obtener una lista de errores comunes que impiden la inscripción y las resoluciones de cada uno.</span><span class="sxs-lookup"><span data-stu-id="98b33-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="98b33-120">[Obtenga información sobre cómo inscribir dispositivos Android en Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="98b33-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
