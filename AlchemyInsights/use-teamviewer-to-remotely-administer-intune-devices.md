---
title: Use TeamViewer para administrar dispositivos Intune de manera remota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798465"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Use TeamViewer para administrar dispositivos Intune de manera remota

Los dispositivos administrados por Intune se pueden administrar de forma remota con [TeamViewer](https://www.teamviewer.com/).

Para administrar Intune con TeamViewer, siga estos pasos: 

Empiece por obtener credenciales de TeamViewer para configurar el conector de TeamViewer en Intune. Esto permite que el administrador introduzca las credenciales en la interfaz de usuario del conector de TeamViewer en Dispositivos, una operación única para establecer el vínculo entre Intune y el servicio TeamViewer.

**Parte 1: iniciar una sesión con un dispositivo remoto**

1. En **Todos los dispositivos**, seleccione el dispositivo en el que desea iniciar una sesión remota.
2. En **... Más**, seleccione **Nueva sesión de asistencia remota**.
3. Seleccione **Sí** para confirmar que desea establecer una sesión remota.
    Después de que el servicio TeamViewer reconozca la solicitud "Inicio de una nueva sesión remota", verá una opción para **Iniciar asistencia remota** en los detalles del panel de Información general (o en Essentials) del dispositivo. Seleccione **Ver más** para expandir el panel y mostrar el estado de Asistencia remota.
4. Seleccione **Iniciar sesión remota** para iniciar la sesión en el lado del administrador.
5. Elija descargar el binario de TeamViewer (Windows) y seleccione **Ejecutar**.<br/>
    **Nota** Puede ignorar cualquier página de explorador web abierta en el sitio web de TeamViewer.

6. Acepte la solicitud para que la aplicación de TeamViewer realice cambios en el dispositivo (solo Windows).
7. Se inicia la aplicación de TeamViewer y se incluye el código de la sesión para autenticar la conexión con el dispositivo remoto.

**Parte 2: dispositivo destino de una sesión remota**

1. Abra el portal de la empresa de Intune.
2. Busque la marca de notificación: "Su administrador de TI solicita el control de este dispositivo para una sesión de asistencia remota" y seleccione la notificación.
3. Elija descargar la aplicación de TeamViewer o confirme la descarga de la aplicación de TeamViewer desde el App Store y seleccione **Ejecutar**.
    **Nota** Puede ignorar cualquier página de explorador web abierta en el sitio web de TeamViewer.

4. Acepte la solicitud para que la aplicación de TeamViewer realice cambios en el dispositivo (solo Windows).
5. Se inicia la aplicación de TeamViewer y se incluye el código de la sesión para autenticar la conexión con el dispositivo remoto.
6. Se le preguntará si desea permitir el inicio de la sesión.

**Nota** Los códigos de sesión generados por el servicio TeamViewer son de uso único. Si pierde la conexión, debe:

1. Cerrar la instancia de la aplicación de TeamViewer en el dispositivo remoto y en la estación de trabajo de administración.
2. Cerrar el portal de la empresa en el dispositivo remoto.
3. Iniciar una nueva "Nueva sesión de asistencia remota" en el portal de administración.
4. Volver a abrir el portal de la empresa en el dispositivo remoto para recibir la nueva notificación.
5. Descargar y abrir la aplicación de TeamViewer en el dispositivo remoto y en la estación de trabajo de administración, como antes.