---
title: Registro duplicado de dispositivo en el portal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678521"
---
# <a name="duplicate-device-record-in-the-portal"></a>Registro duplicado de dispositivo en el portal

Es posible que vea dos registros de un mismo dispositivo en el portal si el dispositivo no ha informado correctamente del estado de administración conjunta en el sitio de Configuration Manager. Para comprobar el estado de administración conjunta de un dispositivo, revise la columna **Administrado conjuntamente** del dispositivo en la consola de Configuration Manager. Si la columna no está visible, puede agregarla haciendo clic con el botón derecho en cualquiera de los encabezados de columna y seleccionándola en la lista.

El valor de administración conjunta tiene que ser **Sí**. Si el valor es **No**, abra el applet de cliente de Configuration Manager en el dispositivo cliente y compruebe la propiedad **Administración conjunta** en la pestaña General.

- Si el valor es **Habilitado**, existen problemas con la comunicación del cliente con el punto de administración. Revise **CcmMessaging.log** en el dispositivo para investigar posibles problemas de conectividad.

- Si el valor es **Deshabilitado** y el dispositivo está inscrito en Intune, revise **CoManagementHandler.log** en el dispositivo para asegurarse de que el dispositivo ha recibido la Directiva de administración conjunta.
