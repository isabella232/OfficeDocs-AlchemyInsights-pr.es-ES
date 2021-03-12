---
title: Uso del acceso condicional con Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737583"
---
# <a name="using-conditional-access-with-intune"></a>Uso del acceso condicional con Intune

El uso del acceso condicional con Intune requiere 3 pasos:

- [Crea una directiva de cumplimiento para definir la configuración que debe cumplirse antes de que el dispositivo se considere compatible. Por ejemplo, un dispositivo debe tener una patilla de al menos 6 dígitos antes de considerarlo compatible.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Cree una directiva de acceso condicional que defina qué recursos se protegen y qué condiciones deben cumplirse para tener acceso a esos recursos. Por ejemplo, un dispositivo debe ser compatible antes de acceder al correo electrónico corporativo.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Asegúrese de que tanto las directivas de cumplimiento como las directivas de acceso condicional están dirigidas a los grupos de usuarios deseados. Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Más información...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
