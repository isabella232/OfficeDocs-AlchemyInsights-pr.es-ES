---
title: Términos que faltan SharePoint almacén de términos en línea
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106449"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Habilitar el cifrado de Bitlocker con Intune

La directiva de Endpoint Protection Intune se puede usar para configurar la configuración de cifrado boitlocker para dispositivos Windows como se describe en : Configuración de Windows10 (y versiones posteriores) para proteger dispositivos con Intune

Debes tener en cuenta que muchos dispositivos más recientes que se ejecutan Windows 10 cifrado de bitlocker automático que se desencadena sin la aplicación de la directiva MDM. Esto puede afectar a la aplicación de la directiva si se configura una configuración no predeterminada. Consulta preguntas más frecuentes para obtener más detalles.


Preguntas más frecuentes: ¿Qué ediciones de Windows el cifrado de dispositivos con la directiva Endpoint Protection usuario?
A: La configuración de Intune Endpoint Protection directiva se implementa mediante el CSP de Bitlocker.  No todas las ediciones ni compilaciones de Windows admiten el CSP de Bitlocker. En este momento Windows editions: Enterprise; Se admiten educación, Enterprise móvil y Professional (a partir de la compilación 1809).




P: Si un dispositivo ya está cifrado con Bitlocker mediante la configuración predeterminada del sistema operativo para el método de cifrado y la intensidad del cifrado (XTS-AES-128) se aplicará una directiva con diferentes configuraciones para desencadenar automáticamente el nuevo cifrado de la unidad con la nueva configuración.

R: No. Para aplicar la nueva configuración de cifrado, primero se debe descifrar la unidad.

Nota Para los dispositivos que se inscriben con Autopilot, el cifrado automático que se produciría durante OOBE no se desencadena hasta que se evalúa la directiva de Intune, que permite usar la configuración basada en directivas en lugar de los valores predeterminados del sistema operativo.




P Si un dispositivo está cifrado como resultado de la aplicación de la directiva de Intune, ¿se descifrará cuando se quite esa directiva?

A: La eliminación de la directiva relacionada con el cifrado NO da como resultado el descifrado de las unidades configuradas.




P: ¿Por qué la directiva de cumplimiento de Intune muestra que mi dispositivo no tiene "Bitlocker habilitado", pero lo es?

A: La configuración "Bitlocker enabled" en la directiva de cumplimiento de Intune usa el Windows de atestación de estado del dispositivo (DHA). Este cliente solo mide el estado del dispositivo en el momento del arranque. Por lo tanto, si un dispositivo no se ha reiniciado desde que se completó el cifrado de bitlocker, el servicio cliente DHA no reportará bitlocker como activo.