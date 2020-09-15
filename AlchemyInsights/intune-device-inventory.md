---
title: Inventario de dispositivos Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667895"
---
# <a name="intune-device-inventory"></a>Inventario de dispositivos Intune

El blade de dispositivos ofrece a los administradores información acerca de los dispositivos que se administran en Intune por cada uno de estos. La información que se muestra incluye: hardware, aplicaciones detectadas, estado de cumplimiento del dispositivo y estado de configuración del dispositivo.

Los datos de inventario para el hardware y las aplicaciones detectadas se recopilan en ciclos de siete días. El informe de las aplicaciones y los elementos de hardware específicos es distinto según el sistema operativo del dispositivo y de si el dispositivo es de propiedad personal o empresarial.

Para más información, consulte [Ver detalles de dispositivos de Intune](https://docs.microsoft.com/intune/device-inventory).

**Preguntas frecuentes**

P: No recibo la lista de inventario completa de las aplicaciones presentes en dispositivos Windows inscritos por Intune. ¿Por qué no?

R: En este momento, solo se muestran las aplicaciones modernas para las PC con Windows 10 que han sido identificadas como dispositivos corporativos. Intune no recopila información sobre las aplicaciones Win32 instaladas en estos dispositivos.

P: ¿Por qué no se recopilan los números de teléfono de todos los dispositivos?

R: Los teléfonos que presentan categoría de dispositivos corporativos en Intune no se identifican con su número de teléfono completo cuando, por ejemplo, se ejecuta un informe de inventario de dispositivos móviles. Los números de teléfono de dispositivos Bring-your-own-device siempre aparecen de forma parcial con asteriscos (****), y solo se muestran los últimos cuatro dígitos.