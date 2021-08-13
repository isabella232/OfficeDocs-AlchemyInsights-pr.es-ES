---
title: Implementación de aplicaciones Win32 de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925902"
---
# <a name="intune-win32-app-deployment"></a>Implementación de aplicaciones Win32 de Intune

Microsoft Intune permite que las aplicaciones Win32, como MSI y .EXE, se implementen en dispositivos con Windows 10. El mecanismo de implementación utilizado requiere que la Extensión de administración de Intune (IME) esté presente en el dispositivo de destino. El IME se instalará automáticamente como resultado de la selección de una implementación de script de PowerShell o de una aplicación Win32 en un usuario o dispositivo.  

También hay un conjunto de requisitos previos que deben cumplirse para poder implementar aplicaciones Win32, entre los que se incluyen:

- Plataformas compatibles: Windows 10 versión 1607 o posterior (versiones Enterprise, Pro y Education).
- Arquitectura compatible: x86 y x64.
- Administración de dispositivos: AAD unido e inscrito automáticamente (incluido el dominio híbrido unido y la directiva de grupo inscrita automáticamente)
- Formato de paquete de la aplicación: archivo .**intunewin** preparado por la [Herramienta de preparación de contenido de Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limitaciones:
    - Tamaño máximo: 8 GB.
    - Arquitectura no compatible: ARM.

Revise el documento "[Agregar, asignar y supervisar una aplicación Win32 en Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para información relacionada con estos pasos.

Los detalles sobre la implementación de aplicaciones de resolución de problemas en Windows, incluidas las aplicaciones Win32, se pueden revisar en los siguientes documentos

- [Solución de problemas de instalación de aplicaciones](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Solución de problemas de aplicaciones de Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)