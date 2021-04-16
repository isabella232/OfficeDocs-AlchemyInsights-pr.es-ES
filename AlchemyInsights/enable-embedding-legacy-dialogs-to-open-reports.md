---
title: Habilitar la incrustación de cuadros de diálogo heredados para abrir informes
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814281"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Habilitar la incrustación de cuadros de diálogo heredados para abrir informes

**Síntoma**

Los usuarios no pueden abrir los informes. "Algo ha fallado. Compruebe los detalles técnicos para obtener más información".

**Causa**

No se pueden cargar los informes en UCI con el error: "El descriptor del formulario es nulo o no está definido". Los informes en UCI aún requieren cuadros de diálogo heredados, por lo que el sistema del cliente debe tener *allowlegacydialogsembedding* habilitado.

**Solución**

1. Vaya a **Configuración > Administración > Configuración del sistema > pestaña General**.

2. Establezca la opción "Habilitar la incrustación de determinados cuadros de diálogo heredados en el cliente unificado del explorador de interfaces" en **Sí**.
