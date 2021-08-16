---
title: Acceso condicional con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069729"
---
# <a name="conditional-access-with-intune"></a>Acceso condicional con Intune

El  **uso del acceso condicional**  con Intune requiere 3 pasos:

- Crea una **directiva de cumplimiento** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir la configuración que debe cumplirse antes de que el dispositivo se considere compatible. Por ejemplo, un dispositivo debe tener una patilla de al menos 6 dígitos antes de considerarlo compatible.
- Cree una **directiva de acceso condicional**  que defina qué recursos se protegen y qué condiciones deben cumplirse para tener acceso a esos recursos.  [Por ejemplo, un](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  dispositivo debe ser compatible antes de acceder al correo electrónico corporativo.
- Asegúrese de **que tanto las directivas de cumplimiento**  como las  **directivas**  de acceso condicional están dirigidas a los grupos de usuarios deseados. Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.

**Vínculos útiles:**

[Introducción al cumplimiento de dispositivos](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solución de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Directiva de solución de problemas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger el correo electrónico (Exchange en línea) del acceso de dispositivos no compatibles, se deben seguir ambos documentos:

1. [Proteger el acceso de correo electrónico desde dispositivos con EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteger el acceso de correo electrónico desde dispositivos que usan clientes de autenticación modernos como Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)