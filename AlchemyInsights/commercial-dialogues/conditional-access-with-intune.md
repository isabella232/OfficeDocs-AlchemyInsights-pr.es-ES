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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005791"
---
# <a name="using-conditional-access-with-intune"></a>Uso del acceso condicional con Intune

El uso del acceso condicional con Intune requiere 3 pasos:

- [Crea una directiva de cumplimiento para definir la configuración que debe cumplirse antes de que el dispositivo se considere compatible. Por ejemplo, un dispositivo debe tener una patilla de al menos 6 dígitos antes de considerarlo compatible.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Cree una directiva de acceso condicional que defina qué recursos se protegen y qué condiciones deben cumplirse para tener acceso a esos recursos. Por ejemplo, un dispositivo debe ser compatible antes de acceder al correo electrónico corporativo.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Asegúrese de que tanto las directivas de cumplimiento como las directivas de acceso condicional están dirigidas a los grupos de usuarios deseados. Esto puede requerir la creación de grupos específicos de usuarios en Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Más información...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
