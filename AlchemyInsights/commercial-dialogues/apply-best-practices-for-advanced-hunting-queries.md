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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930150"
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
