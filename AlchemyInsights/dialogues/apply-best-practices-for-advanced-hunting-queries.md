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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="e8554-102">Aplicar procedimientos recomendados para consultas de búsqueda avanzada</span><span class="sxs-lookup"><span data-stu-id="e8554-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="e8554-103">Para obtener resultados más rápido y evitar tiempos de espera mientras se ejecutan consultas complejas, aplique estos procedimientos recomendados:</span><span class="sxs-lookup"><span data-stu-id="e8554-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="e8554-104">Cuando intente nuevas consultas, use siempre un límite para evitar obtener conjuntos de resultados extremadamente grandes.</span><span class="sxs-lookup"><span data-stu-id="e8554-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="e8554-105">Además, se `count` usa para realizar una evaluación inicial del tamaño del conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="e8554-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="e8554-106">Use los filtros de tiempo primero.</span><span class="sxs-lookup"><span data-stu-id="e8554-106">Use time filters first.</span></span> <span data-ttu-id="e8554-107">Lo ideal es limitar las consultas a siete días.</span><span class="sxs-lookup"><span data-stu-id="e8554-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="e8554-108">Al principio de una consulta, justo después del filtro de tiempo, agregue los filtros esperados para quitar la mayoría de los datos.</span><span class="sxs-lookup"><span data-stu-id="e8554-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="e8554-109">Cuando busque tokens completos, use el `has` operador en lugar de `contains` .</span><span class="sxs-lookup"><span data-stu-id="e8554-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="e8554-110">Ejecute una búsqueda en una columna específica en lugar de en todas las columnas.</span><span class="sxs-lookup"><span data-stu-id="e8554-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="e8554-111">Al unir tablas, primero especifique la tabla con menos filas.</span><span class="sxs-lookup"><span data-stu-id="e8554-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="e8554-112">`project` solo las columnas necesarias de las tablas que se han unido.</span><span class="sxs-lookup"><span data-stu-id="e8554-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="e8554-113">Para obtener más información, vea [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="e8554-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
