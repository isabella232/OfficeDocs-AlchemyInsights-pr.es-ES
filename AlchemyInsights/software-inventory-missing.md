---
title: El inventario de software no se encuentra o no es exacto.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: 191d6ae772dc1b1c6b15071da9c4aca14429cf2db17be6ee0db6b23ea0d29e2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084660"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>El inventario de software no se encuentra o no es exacto.

El inventario de software en la Administración de amenazas y vulnerabilidades (TVM) es una lista de software conocido en su organización con Enumeraciones de plataformas comunes (CPE) oficiales.

Los productos de software sin CPE oficiales no tienen vulnerabilidades publicadas. El inventario también incluye detalles como el nombre del proveedor, el número de debilidades, las amenazas y el número de dispositivos expuestos.

Los cambios del software en los dispositivos normalmente se reflejan en los portales de seguridad en dos horas. Sin embargo, a veces pueden tardar más. Actualmente, no hay ninguna forma de forzar la sincronización: es una evaluación continua.

Si realizó un cambio de software y el cambio no se refleja con precisión en la TVM después de 5 horas, siga estos pasos:

1. Compruebe la sección de evidencia del software para comprender cómo fue detectado el software.
1. Asegúrese de que el software sea compatible. Es posible que el software solo sea visible a nivel del dispositivo, incluso si actualmente no es compatible con la Administración de amenazas y vulnerabilidades. Sin embargo, solo están disponibles los datos limitados.
1. Para obtener información sobre cómo informar la inexactitud desde el portal, consulte [Informar inexactitud](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Nota**: Informar de una inexactitud desde el portal MDE es un canal una sola vía para la ingeniería. Si el problema es urgente, abra un vale de soporte.

Para obtener más información, vea [Inventario de software: Administración de amenazas y vulnerabilidades](/microsoft-365/security/defender-endpoint/tvm-software-inventory).