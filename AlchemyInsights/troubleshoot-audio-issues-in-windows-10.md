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
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833308"
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

**Nota:** Si Windows no encuentra un controlador nuevo, busca uno en el sitio web del fabricante del dispositivo y sigue sus instrucciones.

**Reinstalar el controlador**

Si no puedes actualizar a través del Administrador de dispositivos o encontrar un nuevo controlador en el sitio web del fabricante, prueba estos pasos:

1. En el Administrador de dispositivos, haga clic con el botón secundario (o mantenga presionado) el controlador de audio y seleccione **Desinstalar**. Reinicia el dispositivo y Windows intentará reinstalar el controlador.

2. Si reinstalar el controlador no funciona, prueba a usar el controlador de audio genérico que viene con Windows. En el Administrador de dispositivos, haga clic con el botón secundario (o presione y mantenga presionado) el **controlador** de audio > Actualizar software del controlador Examinar mi equipo en busca de software de controladores Permítanme elegir de una lista de controladores de dispositivo en mi equipo , seleccione Dispositivo de audio de alta definición, seleccione Siguiente y siga las instrucciones para  >    >  instalarlo.  
