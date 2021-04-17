---
title: Solucionar problemas con la inscripción de dispositivos Android en Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830959"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Solucionar problemas con la inscripción de dispositivos Android en Microsoft Intune

Revise los recursos que se enumeran a continuación para resolver el problema ahora.
  
Algunos problemas comunes y pasos de resolución:
  
 **Error de dispositivo no cifrado en el Portal de empresa:** Las versiones más recientes de Android, especialmente a partir de v7.0, requieren un código de acceso de inicio para asegurarse de que el dispositivo está totalmente cifrado. Las soluciones comunes son habilitar un pin de inicio o cifrar completamente el dispositivo. Revise [este documento para](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) obtener más información.
  
 Los dispositivos no pueden realizar la protección con el servicio de Intune o **mostrarse como "Incorrecto" en la consola de administración de Intune:** Es posible que algunos dispositivos Samsung 4.4 y 5.5 no entren en el servicio. Hay 3 soluciones posibles para este problema:
  
1. Abra manualmente la aplicación Portal de empresa de Intune, que iniciará automáticamente una sincronización de dispositivos.

2. Actualiza el dispositivo a Android 6.0 o posterior.

3. Deshabilita a Samsung Smart Manager para que no administre el Portal de empresa de Intune. Revise [este documento para](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) obtener más detalles sobre estos problemas y resoluciones.

 **Tipo de licencia de** usuario Error no válido o Nombre de usuario No **reconocido:** se debe asignar una licencia de Intune o EMS al usuario. Revise estos documentos para asignar una licencia a través de: Centro de administración de Office o Azure Portal.
  
Recursos adicionales para ayudar a resolver el problema:
  
1. Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar y resolver errores comunes de inscripción. Revise [este documento para](https://docs.microsoft.com/intune/help-desk-operators) obtener más detalles.

2. Revise [este documento para](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) obtener una lista de errores comunes que impiden la inscripción y las resoluciones de cada uno.

3. [Obtenga información sobre cómo inscribir dispositivos Android en Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
