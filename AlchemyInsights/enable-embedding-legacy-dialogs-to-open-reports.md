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
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="0e51d-102">Habilitar la incrustación de cuadros de diálogo heredados para abrir informes</span><span class="sxs-lookup"><span data-stu-id="0e51d-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="0e51d-103">**Síntoma**</span><span class="sxs-lookup"><span data-stu-id="0e51d-103">**Symptom**</span></span>

<span data-ttu-id="0e51d-104">Los usuarios no pueden abrir los informes.</span><span class="sxs-lookup"><span data-stu-id="0e51d-104">Users are unable to open reports.</span></span> <span data-ttu-id="0e51d-105">"Algo ha fallado.</span><span class="sxs-lookup"><span data-stu-id="0e51d-105">"Something has gone wrong.</span></span> <span data-ttu-id="0e51d-106">Compruebe los detalles técnicos para obtener más información".</span><span class="sxs-lookup"><span data-stu-id="0e51d-106">Check technical details for more details."</span></span>

<span data-ttu-id="0e51d-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="0e51d-107">**Cause**</span></span>

<span data-ttu-id="0e51d-108">No se pueden cargar los informes en UCI con el error: "El descriptor del formulario es nulo o no está definido".</span><span class="sxs-lookup"><span data-stu-id="0e51d-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="0e51d-109">Los informes en UCI aún requieren cuadros de diálogo heredados, por lo que el sistema del cliente debe tener *allowlegacydialogsembedding* habilitado.</span><span class="sxs-lookup"><span data-stu-id="0e51d-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="0e51d-110">**Solución**</span><span class="sxs-lookup"><span data-stu-id="0e51d-110">**Solution**</span></span>

1. <span data-ttu-id="0e51d-111">Vaya a **Configuración > Administración > Configuración del sistema > pestaña General**.</span><span class="sxs-lookup"><span data-stu-id="0e51d-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="0e51d-112">Establezca la opción "Habilitar la incrustación de determinados cuadros de diálogo heredados en el cliente unificado del explorador de interfaces" en **Sí**.</span><span class="sxs-lookup"><span data-stu-id="0e51d-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
