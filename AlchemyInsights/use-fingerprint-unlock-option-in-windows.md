---
title: Use la opción de desbloqueo de huellas digitales en Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972016"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Use la opción de desbloqueo de huellas digitales en Windows 10

**Habilitar Windows Hello huella digital**

Para desbloquear Windows 10 con la huella digital, debes configurar Windows Hello huella digital agregando (dejando que Windows aprenda a reconocer) al menos un dedo. 

1. Vaya a **Configuración > cuentas > opciones de inicio** de sesión (o haga clic [aquí](ms-settings:signinoptions?activationSource=GetHelp)). Aparecerán las opciones de inicio de sesión disponibles. Por ejemplo:

    ![Opciones de inicio de sesión.](media/sign-in-options.png)

2. Haga clic o pulse **Windows Hello huella** digital y, a continuación, haga clic **en Configurar**. En la ventana Windows Hello configuración, haga clic **en Introducción.** El sensor de huella digital se activará y se te pedirá que coloques el dedo en el sensor:

   ![Sensor de huella digital.](media/fingerprint-sensor.png)

3. Siga las instrucciones, que le pedirán que analice repetidamente el dedo. Cuando esto termine, tendrás la opción de agregar otros dedos que quieras usar para el inicio de sesión. La próxima vez que inicie sesión en Windows 10, tendrá la opción de usar su huella digital para hacerlo.

**Windows Hello Huella digital no disponible como opción de inicio de sesión**

Si Windows Hello Fingerprint no se muestra como una opción en las opciones de inicio de **sesión,** significa que Windows no conoce ningún lector de huellas digitales o escáner conectado al equipo, o que una directiva del sistema impide su uso (si, por ejemplo, el equipo está administrado por su lugar de trabajo). Para solucionar problemas: 

1. Selecciona el **botón Inicio** en la barra de tareas y busca Administrador **de dispositivos**.

2. Haga clic o pulse para abrir **el Administrador de dispositivos**.

3. En el Administrador de dispositivos, expanda Dispositivos biométricos haciendo clic en su galón.

   ![Dispositivos biométricos.](media/biometric-devices.png)

4. El escáner de huellas digitales debe aparecer como un dispositivo biométrico, como el escáner WBDI de Synaptics:

   ![Dispositivos biométricos.](media/biometric-devices-expanded.png)

5. Si no se muestra el escáner de huellas digitales y el escáner está integrado en el equipo, vaya al sitio web del fabricante del equipo. En la sección soporte técnico del modelo de equipo, busque un controlador de Windows 10 para un escáner que pueda instalar.

6. Si el escáner es independiente del equipo (conectado a través de USB), vaya al sitio web del fabricante del escáner para buscar e instalar un software de controlador de dispositivo Windows 10 para el modelo de escáner que tiene.
