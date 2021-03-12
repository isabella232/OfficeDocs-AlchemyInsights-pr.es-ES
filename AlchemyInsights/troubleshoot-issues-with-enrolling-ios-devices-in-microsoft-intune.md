---
title: Solucionar problemas con la inscripción de dispositivos iOS en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708979"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2d683-102">Solucionar problemas con la inscripción de dispositivos iOS en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2d683-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2d683-103">Revise los recursos que se enumeran a continuación para resolver el problema ahora.</span><span class="sxs-lookup"><span data-stu-id="2d683-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2d683-104">Algunos mensajes de error comunes y pasos de resolución:</span><span class="sxs-lookup"><span data-stu-id="2d683-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2d683-105">**Límite de dispositivo alcanzado** El usuario tiene más dispositivos inscritos que el límite de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2d683-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2d683-106">Revise estos documentos para [quitar un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o cambiar el límite del [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2d683-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2d683-107">**Este servicio no es compatible. Sin directiva de inscripción:** el Servicio de notificaciones de inserción de Apple (APNS) debe configurarse o renovarse.</span><span class="sxs-lookup"><span data-stu-id="2d683-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2d683-108">Revise [este documento para](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) obtener instrucciones sobre cómo hacerlo.</span><span class="sxs-lookup"><span data-stu-id="2d683-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2d683-109">**Tipo de licencia de usuario No válido o Nombre de usuario no reconocido:** El usuario debe tener asignada una licencia de Intune o EMS.</span><span class="sxs-lookup"><span data-stu-id="2d683-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2d683-110">Revise estos documentos para asignar una licencia a través de: [Centro de administración de Office](https://docs.microsoft.com/intune/licenses-assign) o Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2d683-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2d683-111">Recursos adicionales para ayudar a resolver el problema:</span><span class="sxs-lookup"><span data-stu-id="2d683-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2d683-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción.</span><span class="sxs-lookup"><span data-stu-id="2d683-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2d683-113">Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles.</span><span class="sxs-lookup"><span data-stu-id="2d683-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2d683-114">Consulte estos documentos para ver una lista de errores comunes que impiden la inscripción y las soluciones para cada uno: [Guía de solución de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) y [Documento de solución de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2d683-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2d683-115">[Obtenga información sobre cómo inscribir dispositivos iOS en Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2d683-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

