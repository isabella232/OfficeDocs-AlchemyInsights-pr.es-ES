---
title: Gráfico que muestra un número diferente de registros en la cuadrícula
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431795"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Gráfico que muestra un número diferente de registros en la cuadrícula

**Síntoma**

En el caso de los gráficos de la página de panel, al hacer clic en el gráfico "..." y hago clic en "Ver registros", se desplaza a la página de la cuadrícula para ver todos los registros. A veces, el número de registros cambia.

**Causa**

Esto se debe a la diferencia de vistas entre el gráfico en la página del panel original y el gráfico en la Página principal de la cuadrícula.  

**Solución**

1. Seleccione la vista de la página original y la vista de la cuadrícula para ver si son diferentes.
2. Cambiar la vista de la cuadrícula para que coincida con la vista en la página original.
3. Si no se encuentra la vista correcta, normalmente significa que la vista no está habilitada en el diseñador de aplicaciones.
4. Vaya al diseñador de aplicaciones de la aplicación específica, elija la entidad y sus vistas, marque la vista que quiera habilitar, guarde, publique y cierre.
5. Actualice la página.