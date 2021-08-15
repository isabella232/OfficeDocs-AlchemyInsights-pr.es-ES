---
title: Solucionar problemas de audio en Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039443"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Solución de problemas de audio en Windows 10

**Ejecutar el solucionador de problemas de audio**

1.  Abra la configuración [de solución de problemas](ms-settings:troubleshoot).

2.  Seleccione **Reproducir audio** Ejecute el  >  **solucionador de problemas**.

**Establecer el dispositivo predeterminado**

Si te conectas a un dispositivo de audio con USB o HDMI, es posible que debas establecer ese dispositivo como predeterminado:

1. Abra **Iniciar**  >  **sonido** y, a continuación, seleccione **Sonido** o **Cambiar sonidos** del sistema en la lista de resultados.

2.  En la **pestaña Reproducción,** seleccione un dispositivo, **seleccione Establecer predeterminado** y, a continuación, seleccione **Aceptar**.

**Comprobar cables, volumen, altavoces y auriculares**

1. Compruebe si hay cables sueltos en las conexiones de altavoces y auriculares y asegúrese de que están conectados al conector correcto.

2. Comprueba los niveles de energía y volumen e intenta activar todos los controles de volumen.

3. Algunos altavoces y aplicaciones tienen sus propios controles de volumen; es posible que deba comprobarlos todos para asegurarse de que están en los niveles correctos.

4. Intente conectarse con un puerto USB diferente.

**Nota:** Recuerde que es posible que los altavoces no funcionen cuando los auriculares están conectados.

**Comprobar administrador de dispositivos**

Para asegurarse de que los controladores están actualizados:

1. Selecciona **Inicio**, escribe **Administrador de** dispositivos y, a continuación, selecciona Administrador **de** dispositivos en la lista de resultados.

2. En **Controladores de sonido, vídeo** y juegos, selecciona tu tarjeta de sonido, ábrala, selecciona la pestaña Controlador y selecciona Actualizar **controlador**. 

**Nota:** si Windows no encuentra un controlador nuevo, busque uno en el sitio web del fabricante del dispositivo y siga sus instrucciones.

**Reinstalar el controlador**

Si no puedes actualizar a través del Administrador de dispositivos o encontrar un nuevo controlador en el sitio web del fabricante, prueba estos pasos:

1. En el Administrador de dispositivos, haga clic con el botón secundario (o mantenga presionado) el controlador de audio y seleccione **Desinstalar**. Reinicie el dispositivo y Windows intentará reinstalar el controlador.

2. Si reinstalar el controlador no funciona, intente usar el controlador de audio genérico que viene con Windows. En el Administrador de dispositivos, haga clic con el botón secundario (o presione y mantenga presionado) el **controlador** de audio > Actualizar software del controlador Examinar mi equipo en busca de software de controladores Permítanme elegir de una lista de controladores de dispositivo en mi equipo , seleccione Dispositivo de audio de alta definición, seleccione Siguiente y siga las instrucciones para  >    >  instalarlo.  
