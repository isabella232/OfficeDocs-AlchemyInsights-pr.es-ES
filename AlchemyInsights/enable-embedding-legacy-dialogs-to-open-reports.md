---
title: Habilitar la incrustación de cuadros de diálogo heredados para abrir informes
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
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806452"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="9eb00-102">Habilitar la incrustación de cuadros de diálogo heredados para abrir informes</span><span class="sxs-lookup"><span data-stu-id="9eb00-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="9eb00-103">**Síntoma**</span><span class="sxs-lookup"><span data-stu-id="9eb00-103">**Symptom**</span></span>

<span data-ttu-id="9eb00-104">Los usuarios no pueden abrir los informes.</span><span class="sxs-lookup"><span data-stu-id="9eb00-104">Users are unable to open reports.</span></span> <span data-ttu-id="9eb00-105">"Algo ha fallado.</span><span class="sxs-lookup"><span data-stu-id="9eb00-105">"Something has gone wrong.</span></span> <span data-ttu-id="9eb00-106">Compruebe los detalles técnicos para obtener más información".</span><span class="sxs-lookup"><span data-stu-id="9eb00-106">Check technical details for more details."</span></span>

<span data-ttu-id="9eb00-107">**Causa**</span><span class="sxs-lookup"><span data-stu-id="9eb00-107">**Cause**</span></span>

<span data-ttu-id="9eb00-108">No se pueden cargar los informes en UCI con el error: "El descriptor del formulario es nulo o no está definido".</span><span class="sxs-lookup"><span data-stu-id="9eb00-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="9eb00-109">Los informes en UCI aún requieren cuadros de diálogo heredados, por lo que el sistema del cliente debe tener *allowlegacydialogsembedding* habilitado.</span><span class="sxs-lookup"><span data-stu-id="9eb00-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="9eb00-110">**Solución**</span><span class="sxs-lookup"><span data-stu-id="9eb00-110">**Solution**</span></span>

1. <span data-ttu-id="9eb00-111">Vaya a **Configuración > Administración > Configuración del sistema > pestaña General**.</span><span class="sxs-lookup"><span data-stu-id="9eb00-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="9eb00-112">Establezca la opción "Habilitar la incrustación de determinados cuadros de diálogo heredados en el cliente unificado del explorador de interfaces" en **Sí**.</span><span class="sxs-lookup"><span data-stu-id="9eb00-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
