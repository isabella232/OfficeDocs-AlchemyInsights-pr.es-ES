---
title: Búsqueda de dispositivos iOS perdidos con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042323"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Búsqueda de dispositivos iOS perdidos con Intune

Habilitar el modo de pérdida en un dispositivo iOS permite a un administrador colocar un mensaje y un número de teléfono de contacto en la pantalla de bloqueo del dispositivo.

Después de habilitar el modo de pérdida, el administrador puede usar la acción Buscar dispositivo para identificar la ubicación física del dispositivo.

La acción Buscar dispositivo en Intune funciona con dispositivos iOS, y muestra la ubicación de un dispositivo específico en un mapa.

El uso de esta acción requiere que el dispositivo iOS esté en:

- Modo supervisado
- Modo de pérdida

Para obtener más información, consulte [Habilitar el modo de pérdida en dispositivos iOS/iPadOS con Intune](https://docs.microsoft.com/intune/device-lost-mode) y [Encontrar dispositivos iOS/iPadOS perdidos o robados, con Intune](https://docs.microsoft.com/intune/device-locate).

**Preguntas frecuentes**

P: He emitido una acción remota para quitar los datos de la empresa de un dispositivo y ahora se ha quedado en estado pendiente.

R: Para que una acción remota tenga efecto de forma correcta, el dispositivo de destino debe tener conexión a Internet y estar en buen estado. En las siguientes situaciones, la acción remota permanece en estado pendiente durante 30 días o hasta que el dispositivo reconozca el comando:

- Cuando el dispositivo no tiene conectividad
- Cuando el dispositivo deja de tener el estado de administración con Intune.

Si cree que un dispositivo ya no está protegido y que no podrá eliminar los datos de la empresa, seleccione Eliminar. La eliminación borra el registro del dispositivo para que ya no aparezca en la lista de dispositivos de Intune. Si el dispositivo se vuelve a activar, el usuario tendrá que volver a inscribirse.

P: ¿Por qué no puedo usar determinadas acciones remotas?

R: No todas las plataformas admiten todas las acciones remotas en dispositivos. Las siguientes acciones remotas son específicas de una plataforma, por lo que solo están disponibles para las plataformas indicadas.

- Deshabilitar Bloqueo de activación (solo iOS)
- Comienzo de cero (solo Windows)
- Modo perdido (solo iOS)
- Buscar dispositivo (solo iOS)
- Reiniciar (solo Windows)

Para obtener más información sobre cada acción, consulte [Acciones de dispositivo disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).