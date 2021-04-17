---
title: Faltan o no se actualizan eventos del calendario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819984"
---
# <a name="calendar-events-missing-or-not-updating"></a>Faltan o no se actualizan eventos del calendario

Si faltan elementos del calendario o no se actualizan, comience por revisar el recuento de elementos en las propiedades de la carpeta Calendario en Outlook: 

1. Haga clic con el botón derecho en la carpeta **Calendario** del usuario afectado y seleccione **Propiedades**.

1. Seleccione la pestaña **Sincronización**.

Si el número de elementos no es el mismo en la carpeta Server y la carpeta Offline:

1.  Seleccione la carpeta **Calendario**.

1.  Vaya a la pestaña **Enviar**/**Recibir** y seleccione **Actualizar carpeta**.

Si aún no se actualiza el calendario o si faltan eventos, descargue la Herramienta de comprobación del calendario para Outlook desde el [centro de descarga de Microsoft](https://www.microsoft.com/download/details.aspx?id=28786). Determine si hay más de 5 000 elementos en la carpeta de calendario, ya que esto puede causar síntomas como que no se actualicen las reuniones de calendario o errores de reunión. 

Para más información, consulte [Problemas de rendimiento de Outlook cuando hay demasiados elementos o carpetas en un modo de almacenamiento en caché de archivos .ost o .pst](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).