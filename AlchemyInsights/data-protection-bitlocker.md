---
title: DataProtection- Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815632"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitar el cifrado de Bitlocker con Intune

La directiva de protección de extremo de Intune se puede usar para configurar la configuración de cifrado de Bitlocker para dispositivos Windows. Para obtener más información, consulta [Configuración de Windows 10 (y versiones posteriores) para proteger dispositivos con Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Además de la directiva de protección de puntos de conexión, también hay un informe de cifrado que proporciona una vista más detallada del estado de cifrado de los dispositivos. Se puede obtener acceso a este informe desde el portal de MEM en **Dispositivos > Monitor** y, a continuación, en **Configuración,** seleccione [Informe de cifrado](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Si encuentras que Bitlocker no se habilita como se esperaba o que el perfil que se usa para habilitar Bitlocker está en un estado de error, revisa el informe de cifrado para comprender mejor por qué se está produciendo el comportamiento.

Para obtener más información sobre cómo interpretar el informe, incluidos los distintos valores de estado de cifrado, consulte [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Debes tener en cuenta que muchos dispositivos más recientes que ejecutan Windows 10 admiten el cifrado de Bitlocker automático, que se desencadena sin la aplicación de la directiva MDM. Esto puede afectar a la aplicación de la directiva si se configuran opciones de configuración no predeterminadas. Consulta las siguientes preguntas más frecuentes para obtener más detalles.

Para obtener información acerca de la solución de problemas de bitlocker, consulte [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Preguntas más frecuentes**

P: ¿Qué ediciones de Windows admiten el cifrado de dispositivos mediante la directiva de endpoint protection?<br>
A: La configuración de la directiva de protección de extremo de Intune se implementa mediante [el CSP de Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). No todas las ediciones o compilaciones de Windows admiten el CSP de Bitlocker. <br><br>

P: ¿Cómo se puede habilitar Bitlocker en dispositivos sin necesidad de la interacción del usuario final?<br>
A: Siempre que se cumplen los requisitos previos necesarios, es posible habilitar Bitlocker "Cifrado silencioso" a través de Intune. Consulta los detalles de los requisitos del dispositivo y la configuración de la directiva de ejemplo para habilitar el cifrado silencioso en el siguiente documento: Habilitar silenciosamente el cifrado [de Bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: Si un dispositivo ya está cifrado con Bitlocker mediante la configuración predeterminada del sistema operativo para el método de cifrado y la intensidad del cifrado (XTS-AES-128), ¿aplicar una directiva con diferentes configuraciones desencadenará automáticamente el nuevo cifrado de la unidad con la nueva configuración?<br>
R: No. Para aplicar la nueva configuración de cifrado, primero se debe descifrar la unidad.<br><br>
**Nota:** Para los dispositivos que se inscriben con Autopilot, el cifrado automático que se produciría durante OOBE no se desencadena hasta que se evalúa la directiva de Intune, lo que permite usar la configuración basada en directivas en lugar de los valores predeterminados del sistema operativo.
 
P: Si un dispositivo está cifrado como resultado de la aplicación de la directiva de Intune, ¿se descifrará cuando se quite esa directiva?<br>
A: La eliminación de la directiva relacionada con el cifrado NO da como resultado el descifrado de las unidades configuradas.
 
P: ¿Por qué la directiva de cumplimiento de Intune muestra que mi dispositivo no tiene Bitlocker habilitado, aunque lo sea?<br>
A: La configuración "Bitlocker enabled" en la Directiva de cumplimiento de Intune usa el cliente de Atestación de estado de dispositivos windows (DHA). Este cliente solo mide el estado del dispositivo en el momento del arranque. Por lo tanto, si un dispositivo no se ha reiniciado desde que se completó el cifrado de Bitlocker, el servicio cliente DHA no notificaría a Bitlocker como activo.
 
 