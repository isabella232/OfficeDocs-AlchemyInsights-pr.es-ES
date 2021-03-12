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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Solucionar problemas con la inscripción de dispositivos iOS en Microsoft Intune

Revise los recursos que se enumeran a continuación para resolver el problema ahora. 
  
Algunos mensajes de error comunes y pasos de resolución:
  
- **Límite de dispositivo alcanzado** El usuario tiene más dispositivos inscritos que el límite de dispositivos. Revise estos documentos para [quitar un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o cambiar el límite del [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Este servicio no es compatible. Sin directiva de inscripción:** el Servicio de notificaciones de inserción de Apple (APNS) debe configurarse o renovarse. Revise [este documento para](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) obtener instrucciones sobre cómo hacerlo. 
    
- **Tipo de licencia de usuario No válido o Nombre de usuario no reconocido:** El usuario debe tener asignada una licencia de Intune o EMS. Revise estos documentos para asignar una licencia a través de: [Centro de administración de Office](https://docs.microsoft.com/intune/licenses-assign) o Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Recursos adicionales para ayudar a resolver el problema:
  
1. Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción. Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles. 
    
2. Consulte estos documentos para ver una lista de errores comunes que impiden la inscripción y las soluciones para cada uno: [Guía de solución de problemas](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) y [Documento de solución de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Obtenga información sobre cómo inscribir dispositivos iOS en Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

