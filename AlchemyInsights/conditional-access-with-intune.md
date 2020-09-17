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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807676"
---
# <a name="conditional-access-with-intune"></a>Acceso condicional con Intune

El uso de  **acceso condicional**  con Intune requiere 3 pasos:

- Cree una  **Directiva de cumplimiento**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) para definir la configuración que se debe cumplir antes de que el dispositivo se considere conforme. Por ejemplo, un dispositivo debe tener un PIN de al menos 6 dígitos antes de que se considere compatible.
- Cree una **Directiva de acceso condicional**  que defina los recursos que se van a proteger y las condiciones que deben cumplirse para obtener acceso a esos recursos.  [Por ejemplo,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispositivo debe ser compatible antes de obtener acceso al correo electrónico corporativo.
- Asegúrese de que las directivas de **cumplimiento**  y  **las directivas de acceso condicional**  estén dirigidas a los grupos de usuarios deseados. Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.

**Vínculos útiles:**

[Introducción al cumplimiento de dispositivos](https://docs.microsoft.com/intune/device-compliance-get-started)

[Solución de problemas de CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Directiva de solución de problemas](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Para proteger el correo electrónico (Exchange Online) del acceso de dispositivos no compatibles, se deben seguir ambos documentos:

1. [Proteger el acceso al correo electrónico de dispositivos con EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteger el acceso al correo electrónico desde dispositivos con clientes de autenticación modernos como Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)