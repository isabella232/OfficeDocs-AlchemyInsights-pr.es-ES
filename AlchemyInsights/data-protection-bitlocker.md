---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778210"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitar el cifrado de BitLocker con Intune

La directiva de Endpoint Protection de Intune se puede usar para configurar las opciones de cifrado de BitLocker para dispositivos Windows. Para obtener más información, consulta [la configuración de Windows 10 (y](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)versiones posteriores) para proteger dispositivos con Intune.

Además de la directiva de Endpoint Protection, también hay un informe de cifrado que proporciona una vista más detallada del estado de cifrado de los dispositivos. Se puede obtener acceso a este informe desde el portal de MEM en Dispositivos **> Monitor** y, a continuación, en **Configuración,** seleccione Informe [de cifrado.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Si ves que Bitlocker no se puede habilitar como se esperaba o que el perfil que se usa para habilitar Bitlocker está en un estado de error, revisa el informe de cifrado para comprender mejor por qué se está produciendo el comportamiento.

Para obtener información detallada sobre cómo interpretar el informe, incluidos los distintos valores de estado de cifrado, vea Supervisar el cifrado [de dispositivos con Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Debes tener en cuenta que muchos dispositivos más recientes que ejecutan Windows 10 admiten el cifrado de BitLocker automático, que se desencadena sin la aplicación de la directiva MDM. Esto puede afectar a la aplicación de la directiva si se configuran opciones no predeterminadas. Consulte las siguientes preguntas más frecuentes para obtener más información.

Para obtener información sobre cómo solucionar problemas de BitLocker, consulta [Solucionar problemas de directivas de BitLocker en Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Preguntas frecuentes**

P: ¿Qué ediciones de Windows admiten el cifrado de dispositivos con la directiva de Endpoint Protection?<br>
A: La configuración de la directiva de Endpoint Protection de Intune se implementa con el [CSP de BitLocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) No todas las ediciones o compilaciones de Windows admiten el CSP de BitLocker. <br><br>

P: ¿Cómo se puede habilitar BitLocker en dispositivos sin necesidad de interacción del usuario final?<br>
A: Siempre que se cumplen los requisitos previos necesarios, es posible habilitar el "Cifrado silencioso" de BitLocker a través de Intune. Consulta los detalles de los requisitos del dispositivo y la configuración de directivas de ejemplo para habilitar el cifrado silencioso en el siguiente documento: Habilitar silenciosamente el cifrado [de Bitlocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

P: Si un dispositivo ya está cifrado con BitLocker con la configuración predeterminada del sistema operativo para el método de cifrado y la intensidad de cifrado (XTS-AES-128), ¿se aplicará una directiva con diferentes configuraciones automáticamente que desencadenará el nuevo cifrado de la unidad con la nueva configuración?<br>
R: No. Para aplicar la nueva configuración de cifrado, primero se debe descifrar la unidad.<br><br>
**Nota:** Para los dispositivos que se inscriben con Autopilot, el cifrado automático que se produciría durante la OOBE no se desencadena hasta que se evalúa la directiva de Intune, lo que permite usar la configuración basada en directivas en lugar de los valores predeterminados del sistema operativo.
 
P: Si un dispositivo está cifrado como resultado de la aplicación de la directiva de Intune, ¿se descifrará cuando se quite esa directiva?<br>
A: La eliminación de la directiva relacionada con el cifrado NO da como resultado el descifrado de las unidades configuradas.
 
P: ¿Por qué la directiva de cumplimiento de Intune muestra que mi dispositivo no tiene BitLocker habilitado, aunque lo sea?<br>
A: La configuración "Bitlocker habilitado" en la directiva de cumplimiento de Intune usa el cliente de Atestación de estado de dispositivos Windows (DHA). Este cliente solo mide el estado del dispositivo durante el arranque. Por lo tanto, si un dispositivo no se ha reiniciado desde que se completó el cifrado de BitLocker, el servicio cliente DHA no mostrará BitLocker como activo.
 
 