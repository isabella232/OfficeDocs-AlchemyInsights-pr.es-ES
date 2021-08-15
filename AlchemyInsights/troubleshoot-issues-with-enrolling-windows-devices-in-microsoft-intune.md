---
title: Solucionar problemas con la inscripción de Windows dispositivos en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981058"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Solucionar problemas con la inscripción de Windows dispositivos en Microsoft Intune

Revise los recursos que se enumeran a continuación para resolver el problema ahora.
  
Algunos mensajes de error comunes y pasos de resolución:
  
 **El software no se puede instalar, 0x80cf4017:** El certificado de cuenta ha expirado. Vuelva a descargar el paquete de software cliente de PC en la Consola de administración de Intune. Revise esta documentación para obtener más información.
  
 **Código de error 0x801c0003:** El error puede producirse en los siguientes escenarios:
  
-  El usuario tiene más dispositivos inscritos que el límite de dispositivos. Revise estos documentos para [quitar un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o cambiar el límite del [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Los usuarios pueden unir dispositivos a Azure AD" se establece en "ninguno". Estadeselo en todos o seleccione usuarios. Revise [esta documentación](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para obtener más información.

-  El dispositivo ya está inscrito por otro usuario. Si ese es el caso, quita el dispositivo de la consola de Azure Intune o desenrolla manualmente el dispositivo antes de volver a intentarlo.

-  El dispositivo está Windows 10 Home. Solo Windows 10 Pro, Educación y Enterprise SKU pueden unirse a Azure Active Directory.

Recursos adicionales para ayudar a resolver el problema:
  
-  Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción. Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles.

-  Consulte estos documentos para ver una lista de errores comunes que impiden la inscripción y las soluciones para cada uno: [Guía de solución de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) y [Documento de solución de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Obtenga información sobre cómo inscribir Windows dispositivos en Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
