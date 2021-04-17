---
title: Solución de problemas del monitor existente
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824596"
---
# <a name="troubleshoot-an-existing-monitor"></a>Solucionar problemas de un monitor existente

Pruebe estas soluciones para solucionar problemas de un monitor. 

**Actualice la pantalla del monitor:**

Presione las siguientes teclas al mismo tiempo: Tecla Windows + Ctrl + Mayús + B. Esto actualizará la comunicación con el controlador de gráficos. Los monitores parpadearán momentáneamente y volverán después de unos segundos.

**Solucionar problemas de hardware de monitor:**

1. Desconecte el cable que conecta el PC al monitor y vuelva a conectarlo.
2. Desconecte los dispositivos no esenciales del PC (como adaptadores o docks).

**Si has instalado recientemente una actualización en el equipo, puedes revertir el controlador de pantalla:**

1. Selecciona **Inicio**, escribe **Administrador de** dispositivos y selecciona Administrador de **dispositivos** en los resultados.
2. Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Propiedades**.
3. Vaya a la **pestaña Controlador** y seleccione **Revertir controlador**. <br>
Nota: Si no está disponible o está atenuado, seleccione **No** en las opciones siguientes para pasar al siguiente paso.
4. Es posible que deba reiniciar el equipo antes de que estos cambios sumen efecto.

**Desinstale y vuelva a instalar el controlador de pantalla:**

1. Selecciona **Inicio**, escribe **Administrador de** dispositivos y selecciona Administrador de **dispositivos** en los resultados.
2. Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Desinstalar dispositivo**. 
3. Seleccione el cuadro situado junto **a Eliminar el software del controlador para este dispositivo** y seleccione **Desinstalar**.<br>
Nota: Es posible que se te pida que reinicies el equipo en esta fase. Asegúrese de escribir las instrucciones restantes antes de reiniciar.
4. Abre el Administrador de dispositivos de nuevo.
5. Expanda la **sección Adaptadores de** pantalla, haga clic con el botón secundario en el adaptador de pantalla y seleccione **Actualizar controlador**.
6. Seleccione **Buscar automáticamente el software del controlador de actualización** y siga las instrucciones de instalación.