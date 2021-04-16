---
title: Registro duplicado de dispositivo en el portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814533"
---
# <a name="duplicate-device-record-in-the-portal"></a>Registro duplicado de dispositivo en el portal

Es posible que vea dos registros de un mismo dispositivo en el portal si el dispositivo no ha informado correctamente del estado de administración conjunta en el sitio de Configuration Manager. Para comprobar el estado de administración conjunta de un dispositivo, revise la columna **Administrado conjuntamente** del dispositivo en la consola de Configuration Manager. Si la columna no está visible, puede agregarla haciendo clic con el botón derecho en cualquiera de los encabezados de columna y seleccionándola en la lista.

El valor de administración conjunta tiene que ser **Sí**. Si el valor es **No**, abra el applet de cliente de Configuration Manager en el dispositivo cliente y compruebe la propiedad **Administración conjunta** en la pestaña General.

- Si el valor es **Habilitado**, existen problemas con la comunicación del cliente con el punto de administración. Revise **CcmMessaging.log** en el dispositivo para investigar posibles problemas de conectividad.

- Si el valor es **Deshabilitado** y el dispositivo está inscrito en Intune, revise **CoManagementHandler.log** en el dispositivo para asegurarse de que el dispositivo ha recibido la Directiva de administración conjunta.
