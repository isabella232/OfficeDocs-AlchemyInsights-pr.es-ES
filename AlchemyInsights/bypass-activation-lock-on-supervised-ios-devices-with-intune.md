---
title: Deshabilitar el bloqueo de activación en dispositivos iOS controlados con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397761"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Deshabilitar el bloqueo de activación en dispositivos iOS controlados con Intune

La capacidad de deshabilitar el bloqueo de activación en dispositivos iOS facilita la recuperación en el caso en que un usuario habilite el bloqueo de activación en un dispositivo corporativo, y luego abandone la empresa.

Los requisitos previos para deshabilitar un bloqueo de activación son los siguientes:

- Un dispositivo que se "supervisa".
- El bloqueo de activación se habilitó correctamente con la directiva de restricción de dispositivos iOS en Intune.

Asimismo, al deshabilitar un bloqueo de activación, debe:

- Poseer físicamente el dispositivo que se va a borrar.
- Copiar el código antes de emitir el borrado.

**Nota:** el código de borrado no distingue entre mayúsculas y minúsculas, por lo que los caracteres "-" no son necesarios.

Para obtener más información, consulte [Deshabilitar el bloqueo de activación en dispositivos iOS supervisados con Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Preguntas frecuentes**

P: **He emitido una acción remota para quitar los datos de la empresa de un dispositivo y ahora está atascado en un estado pendiente.**

R: Para que una acción remota finalice correctamente, el dispositivo de destino tiene que estar conectado y en buen estado. En las siguientes situaciones, la acción remota permanece en un estado pendiente durante 30 días o hasta que el dispositivo reconozca el comando cuando:

- No tiene conectividad.
- Pierde su estado de administración con Intune.

Si cree que un dispositivo ya no se está comprobando, y que no se quitarán los datos de la empresa, seleccione Eliminar. La eliminación quita el registro del dispositivo para que ya no aparezca en la lista de dispositivos de Intune. Para volver a activar el dispositivo, el usuario debe volverlo a inscribir.

P: **¿Por qué no puedo usar determinadas acciones remotas?**

R: No todas las plataformas admiten todas las acciones remotas en dispositivos. Las siguientes acciones remotas son específicas para cada plataforma.

- Deshabilitar Bloqueo de activación (solo iOS)
- Comienzo de cero (solo Windows)
- Modo perdido (solo iOS)
- Buscar dispositivo (solo iOS)
- Reiniciar (solo Windows)

Para obtener más información sobre cada acción, consulte [Acciones de dispositivo disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).