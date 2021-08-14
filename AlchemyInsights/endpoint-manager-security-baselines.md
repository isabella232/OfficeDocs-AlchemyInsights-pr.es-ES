---
title: Administrador de extremos - Líneas de base de seguridad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978178"
---
# <a name="endpoint-manager---security-baselines"></a>Administrador de extremos - Líneas de base de seguridad

Las líneas de base de seguridad son grupos preconfigurados de opciones de configuración de Windows que le ayudarán a aplicar las configuraciones de seguridad recomendadas por los equipos de seguridad correspondientes. Estas líneas de base se pueden personalizar para ofrecer solo la configuración y los valores deseados. Para obtener más información acerca de las líneas base de seguridad, vea [Usar líneas de base de seguridad para configurar dispositivos con Windows 10 en Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Actualmente hay líneas base para estos productos:

- Configuración de seguridad de Windows MDM
- Microsoft Defender para punto de conexión de seguridad
- Microsoft Edge

Cada una de las líneas de base se actualiza periódicamente y se libera en versiones incrementales. Cada versión agrega y quita la configuración de la versión anterior para asegurarse de que la línea de base cumple las instrucciones actuales. La consola de líneas de base de seguridad en punto de conexión de seguridad permite comparar diferentes versiones haciendo visibles los cambios de una versión a otra.

Para obtener instrucciones sobre cómo cambiar de manera más eficaz la versión de línea de base que se implementa, vea [Administrar perfiles de línea de base de seguridad en Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Después de implementar una línea base de seguridad, puede supervisar el estado de implementación y revisar la configuración en cada dispositivo.

**Nota:** Los datos de informes para líneas de base pueden tardar hasta 24 horas en aparecer desde la implementación inicial a un dispositivo y hasta 6 horas para obtener más actualizaciones. 

La causa más común de que no se aplique una configuración de línea de base es porque la misma configuración se usa en un perfil diferente. Para investigar este escenario para un dispositivo específico, seleccione ese dispositivo desde el nodo Estado del dispositivo del perfil de Línea de base de seguridad. Para ver los detalles, consulte [Resolver conflictos de líneas de base de seguridad](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).