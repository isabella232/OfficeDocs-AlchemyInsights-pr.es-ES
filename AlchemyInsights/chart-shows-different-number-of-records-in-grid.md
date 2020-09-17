---
title: Gráfico que muestra un número diferente de registros en la cuadrícula
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793775"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="f59ae-102">Gráfico que muestra un número diferente de registros en la cuadrícula</span><span class="sxs-lookup"><span data-stu-id="f59ae-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="f59ae-103">**Síntoma**</span><span class="sxs-lookup"><span data-stu-id="f59ae-103">**Symptom**</span></span>

<span data-ttu-id="f59ae-104">En el caso de los gráficos de la página de panel, al hacer clic en el gráfico "..." y hago clic en "Ver registros", se desplaza a la página de la cuadrícula para ver todos los registros. A veces, el número de registros cambia.</span><span class="sxs-lookup"><span data-stu-id="f59ae-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="f59ae-105">**Causa**</span><span class="sxs-lookup"><span data-stu-id="f59ae-105">**Cause**</span></span>

<span data-ttu-id="f59ae-106">Esto se debe a la diferencia de vistas entre el gráfico en la página del panel original y el gráfico en la Página principal de la cuadrícula.</span><span class="sxs-lookup"><span data-stu-id="f59ae-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="f59ae-107">**Solución**</span><span class="sxs-lookup"><span data-stu-id="f59ae-107">**Solution**</span></span>

1. <span data-ttu-id="f59ae-108">Seleccione la vista de la página original y la vista de la cuadrícula para ver si son diferentes.</span><span class="sxs-lookup"><span data-stu-id="f59ae-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="f59ae-109">Cambiar la vista de la cuadrícula para que coincida con la vista en la página original.</span><span class="sxs-lookup"><span data-stu-id="f59ae-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="f59ae-110">Si no se encuentra la vista correcta, normalmente significa que la vista no está habilitada en el diseñador de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="f59ae-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="f59ae-111">Vaya al diseñador de aplicaciones de la aplicación específica, elija la entidad y sus vistas, marque la vista que quiera habilitar, guarde, publique y cierre.</span><span class="sxs-lookup"><span data-stu-id="f59ae-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="f59ae-112">Actualice la página.</span><span class="sxs-lookup"><span data-stu-id="f59ae-112">Refresh the page.</span></span>