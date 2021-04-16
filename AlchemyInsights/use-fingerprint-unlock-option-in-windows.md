---
title: Usar la opción de desbloqueo de huellas digitales en Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796694"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Usar la opción de desbloqueo de huellas digitales en Windows 10

**Habilitar Huella digital de Windows Hello**

Para desbloquear Windows 10 con tu huella digital, debes configurar Windows Hello Fingerprint agregando (dejando que Windows aprenda a reconocer) al menos un dedo. 

1. Ve a **Configuración > cuentas > opciones de inicio** de sesión (o haz clic [aquí).](ms-settings:signinoptions?activationSource=GetHelp) Aparecerán las opciones de inicio de sesión disponibles. Por ejemplo:

    ![Opciones de inicio de sesión.](media/sign-in-options.png)

2. Haz clic o pulsa **en Huella digital de Windows Hello** y, a continuación, haz clic en **Configurar**. En la ventana de instalación de Windows Hello, haga clic **en Introducción.** El sensor de huella digital se activará y se te pedirá que coloques el dedo en el sensor:

   ![Sensor de huella digital.](media/fingerprint-sensor.png)

3. Siga las instrucciones, que le pedirán que analice repetidamente el dedo. Cuando esto termine, tendrás la opción de agregar otros dedos que quieras usar para el inicio de sesión. La próxima vez que inicies sesión en Windows 10, tienes la opción de usar la huella digital para hacerlo.

**Huella digital de Windows Hello no está disponible como opción de inicio de sesión**

Si la huella digital de Windows Hello no se muestra como una opción en las opciones de inicio de **sesión,** significa que Windows no conoce ningún lector de huellas digitales o escáner conectado al equipo, o que una directiva del sistema impide su uso (si, por ejemplo, el equipo está administrado por su lugar de trabajo). Para solucionar problemas: 

1. Selecciona el **botón Inicio** en la barra de tareas y busca Administrador **de dispositivos**.

2. Haga clic o pulse para abrir **el Administrador de dispositivos**.

3. En el Administrador de dispositivos, expanda Dispositivos biométricos haciendo clic en su galón.

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. El escáner de huellas digitales debe aparecer como un dispositivo biométrico, como el escáner WBDI de Synaptics:

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. Si no se muestra el escáner de huellas digitales y el escáner está integrado en el equipo, vaya al sitio web del fabricante del equipo. En la sección soporte técnico del modelo de pc, busca un controlador de Windows 10 para un escáner que puedas instalar.

6. Si el escáner es independiente del equipo (conectado a través de USB), vaya al sitio web del fabricante del escáner para buscar e instalar el software del controlador de dispositivo de Windows 10 para el modelo de escáner que tiene.
