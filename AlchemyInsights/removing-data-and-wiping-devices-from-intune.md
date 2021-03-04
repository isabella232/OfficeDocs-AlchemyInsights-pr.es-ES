---
title: Eliminación de datos y borrado de dispositivos desde Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416330"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Eliminación de datos y borrado de dispositivos desde Intune

Las acciones remotas de eliminación y borrado de dispositivos se pueden usar para eliminar los datos de una empresa administrados por Intune, o para realizar un restablecimiento de fábrica y regresar al dispositivo a su configuración predeterminada.

1. Inicie sesión en Administración de dispositivos de Microsoft 365 y diríjase a **Dispositivos** > **Todos los dispositivos**.
2. Seleccione el dispositivo que desea quitar.
3. Seleccione el tipo de eliminación remota que desea realizar. La acción Eliminación solo borra la información de la organización, mientras que el borrado completo restaura el dispositivo a su configuración de fábrica.
4. Seleccione **Sí** para confirmar. Hasta que la eliminación finalice, el estado de la acción del dispositivo se mostrará como *Eliminación pendiente*.
    Cuando se haya completado esta acción, ya no verá el dispositivo móvil en la lista de dispositivos administrados.

> [!NOTE]
> Los datos de la empresa no se pueden eliminar de los dispositivos CONECTADOS a Azure AD. 

Para obtener todos los detalles del efecto de las acciones Retirar y Borrar, incluido lo que se conserva y lo que se elimina, vea la documentación siguiente:

- [Quite dispositivos mediante el borrado, retirada o desenrollando manualmente el](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Cómo borrar solo los datos corporativos desde aplicaciones administradas por Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Borrar todos los datos desde un dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).