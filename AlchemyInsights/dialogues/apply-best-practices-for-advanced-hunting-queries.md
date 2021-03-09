---
title: Aplicar procedimientos recomendados para consultas de búsqueda avanzada
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568720"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Aplicar procedimientos recomendados para consultas de búsqueda avanzada

Para obtener resultados más rápido y evitar tiempos de espera mientras se ejecutan consultas complejas, aplique estos procedimientos recomendados:

- Cuando intente nuevas consultas, use siempre un límite para evitar obtener conjuntos de resultados extremadamente grandes. Además, se `count` usa para realizar una evaluación inicial del tamaño del conjunto de resultados.
- Use los filtros de tiempo primero. Lo ideal es limitar las consultas a siete días.
- Al principio de una consulta, justo después del filtro de tiempo, agregue los filtros esperados para quitar la mayoría de los datos.
- Cuando busque tokens completos, use el `has` operador en lugar de `contains` .
- Ejecute una búsqueda en una columna específica en lugar de en todas las columnas.
- Al unir tablas, primero especifique la tabla con menos filas.
- `project` solo las columnas necesarias de las tablas que se han unido.

Para obtener más información, vea [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).
