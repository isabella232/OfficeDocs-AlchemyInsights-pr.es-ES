---
title: Eliminación de datos y borrado de dispositivos desde Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434632"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Eliminación de datos y borrado de dispositivos desde Intune

Las acciones remotas de eliminación y borrado de dispositivos se pueden usar para eliminar los datos de una empresa administrados por Intune, o para realizar un restablecimiento de fábrica y regresar al dispositivo a su configuración predeterminada.

1. Inicie sesión en Administración de dispositivos de Microsoft 365 y diríjase a **Dispositivos** > **Todos los dispositivos**.
2. Seleccione el dispositivo que desea quitar.
3. Seleccione el tipo de eliminación remota que desea realizar. La acción Eliminación solo borra la información de la organización, mientras que el borrado completo restaura el dispositivo a su configuración de fábrica.
4. Seleccione **Sí** para confirmar. Hasta que la eliminación finalice, el estado de la acción del dispositivo se mostrará como Eliminación pendiente.</br>
    Cuando se complete la acción, ya no verá el dispositivo móvil en la lista de dispositivos administrados.

**Nota** Los datos de la empresa no se pueden eliminar de los dispositivos CONECTADOS a Azure AD.

Para obtener información detallada sobre el efecto de las acciones de eliminación y borrado, incluido lo que se conserva y lo que se elimina, consulte [Eliminar dispositivos con la función borrado, eliminación, o anular la inscripción en el dispositivo de forma manual](https://docs.microsoft.com/intune/devices-wipe).

Para borrar todos los datos de un dispositivo macOS, consulte [Borrar todos los datos de un dispositivo macOS](https://docs.microsoft.com/intune/device-erase).