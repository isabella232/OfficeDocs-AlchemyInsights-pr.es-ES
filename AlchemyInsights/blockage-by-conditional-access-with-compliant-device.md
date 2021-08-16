---
title: El Acceso condicional con dispositivos compatibles me bloquea
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019165"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>El Acceso condicional con dispositivos compatibles me bloquea

**Herramientas altamente recomendadas**

- [Herramienta solucionador de problemas de registro de dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) : una herramienta completa que ayuda a solucionar los problemas de registro de dispositivos más comunes.
- [Script de conectividad de registro de dispositivos de prueba](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : una herramienta que se usa para asegurarse de que un dispositivo puede tener acceso a los puntos de conexión de Registro de dispositivos en la cuenta del sistema.
- [Script de limpieza de dispositivos de Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : una herramienta usada para buscar y administrar dispositivos obsoletos en su entorno.

Estas son algunas de las razones comunes por las que puede producirse un error de Acceso condicional en un dispositivo compatible o por qué los usuarios pueden recibir un mensaje de **No puede llegar al destino desde aquí** durante una solicitud de inicio de sesión a un recurso de la organización.

1. **El dispositivo no está en un estado de dispositivo requerido con un MDM**:

Valide que el dispositivo esté inscrito con un proveedor de MDM aprobado como Intune y esté *marcado como compatible*. Para obtener más información sobre Intune, consulte este [documento](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Para obtener una descripción más clara del cumplimiento de dispositivos e Intune, consulte [usar la directiva de cumplimiento para establecer reglas para los dispositivos que administra con Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Si tiene problemas al inscribir un dispositivo con Intune, encuentre los detalles para la solución de problemas en [Solucionar problemas de inscripción de dispositivos en Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Para obtener más soporte de Intune, cree una solicitud de soporte técnico. Para hacerlo, visite la [página de Ayuda y soporte técnico de Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **El dispositivo no está unido a la red de la organización**:

Para obtener acceso a los recursos de la organización, el dispositivo tiene que estar conectado a la red de la organización, ya sea a través de una conexión directa o una red privada virtual (VPN), y también debe estar unido a una red local o Azure Active Directory. Para unir un dispositivo de trabajo a la red de la organización, vea [Unir el dispositivo de trabajo a la red de su organización](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Para registrar un dispositivo personal/BYOD, vea [Registrar su dispositivo personal en la red de su organización](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Para validar si el dispositivo se ha unido a la red, puede seguir los pasos para dispositivos registrados [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) o para dispositivos de trabajo [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Para localizar el problema de conectividad de red de la organización, siga las siguientes instrucciones:

    1. Inicie sesión en Windows con su cuenta del trabajo o de la escuela,  por ejemplo, alain@contoso.com.
    2. Conéctese a la red de su organización a través de una VPN o DirectAccess.
    3. Después de conectarse, pulse la **Tecla del logotipo de Windows+L** para bloquear el dispositivo.
    4. Desbloquee el dispositivo con su cuenta profesional o educativa y, a continuación, intente obtener acceso a la aplicación o el servicio problemático nuevamente.

Si ve el mensaje de error **No puede llegar al destino desde aquí** de nuevo, es probable que el problema esté en otro lugar.

3. **El sistema operativo no es compatible**:

Asegúrese de que ejecuta una versión compatible del sistema operativo, que incluye:

- **Cliente de Windows**: Windows 7 o versiones posteriores

- **Windows Server**: Windows Server 2008 R2 o posteriores

- **macOS**: macOS X o posteriores

- **Android e iOS**: Última versión de los sistemas operativos móviles de Android e iOS

4. **El explorador web no es compatible**:

Encontrará los exploradores admitidos a continuación. Para la compatibilidad de Chrome con Windows 1703 o versiones posteriores, se necesita una extensión de cuentas de Windows 10. Para Edge 85+, es necesario que el usuario haya iniciado sesión para transmitir correctamente la información de cumplimiento del dispositivo. Para obtener más información, consulte [aquí](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Obtenga más información sobre el mensaje **No puede llegar al destino desde aquí** y los pasos de solución de problemas [aquí](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
