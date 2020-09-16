---
title: Solucionar problemas de Bluetooth en Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730176"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Solucionar problemas de Bluetooth en Windows 10

Si falta el icono de Bluetooth o si no se puede activar o desactivar el Bluetooth, es posible que quiera ejecutar el solucionador de problemas de Bluetooth. [Abra la configuración de solución de problemas](ms-settings:troubleshoot), haga clic en **Bluetooth** , en **Buscar y solucionar otros problemas**, haga clic en **ejecutar el solucionador de problemas**.

Si no ve el icono de Bluetooth, pero Bluetooth aparece en el administrador de dispositivos:

1. En el administrador de dispositivos, haga clic en **Bluetooth**. Mantén presionado (o haz clic con el botón derecho) en el nombre del adaptador Bluetooth y haz clic en **desinstalar dispositivo**.

2. Apaga el dispositivo Windows, espera unos segundos y, a continuación, vuelve a encenderlo. Windows intentará reinstalar el controlador.

Si has instalado recientemente actualizaciones de Windows 10 o actualizado a Windows 10, es posible que quieras comprobar las actualizaciones de los controladores:

1. En el administrador de dispositivos, haga clic en **Bluetooth**y, a continuación, haga clic en el nombre del adaptador Bluetooth (que puede incluir la palabra "radio").

2. Mantén presionado (o haz clic con el botón derecho) en el adaptador Bluetooth y, a continuación, haz clic en **Actualizar**  >  **búsqueda de controlador automáticamente para el software de controlador actualizado**. Siga los pasos y, a continuación, haga clic en **cerrar**.

      - Si Windows no encuentra un nuevo controlador Bluetooth, visita el sitio web del fabricante del equipo y descarga el controlador Bluetooth más reciente desde allí.

    - Una vez descargado, haga clic en **Actualizar controlador**buscar en el  >  **equipo para el software de controlador**  >  **Busque** la ubicación en la que se almacenan los archivos del controlador > **Aceptar**  >  **Next**y siga los pasos para instalar.

3. Después de instalar el controlador actualizado, reinicie el equipo y, a continuación, compruebe si se ha corregido el problema de conexión.

Para obtener más información sobre cómo solucionar problemas de Bluetooth, vea el artículo completo, [solucionar problemas de Bluetooth en Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
