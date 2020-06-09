---
title: 'Error: las reglas de este equipo no coinciden'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618030"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="c7da2-102">Error: las reglas de este equipo no coinciden</span><span class="sxs-lookup"><span data-stu-id="c7da2-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="c7da2-103">Para ver el estado actualizado de este problema conocido, consulte las [reglas de este equipo no coinciden con las reglas de Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="c7da2-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="c7da2-104">El equipo de Outlook ha implementado una corrección en la compilación 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="c7da2-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="c7da2-105">La corrección ya está en una hora de Insider rápida y se dirigirá a la canal mensual en el 2020 de junio de junio.</span><span class="sxs-lookup"><span data-stu-id="c7da2-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="c7da2-106">Una vez que tenga la compilación fija, puede que reciba el mensaje "¿qué reglas desea mantener" una última vez.</span><span class="sxs-lookup"><span data-stu-id="c7da2-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="c7da2-107">Elija servidor cuando se le solicite y, a continuación, vuelva a Outlook y vuelva a habilitar las reglas que se hayan deshabilitado.</span><span class="sxs-lookup"><span data-stu-id="c7da2-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="c7da2-108">Hasta que la corrección esté disponible, use la siguiente solución alternativa:</span><span class="sxs-lookup"><span data-stu-id="c7da2-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="c7da2-109">**Solución**: en informes recientes, el problema se debe a aquellos que solo han creado reglas de cliente en el escritorio de Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7da2-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="c7da2-110">Si sigue teniendo el problema, considere la posibilidad de eliminar las reglas y, a continuación, cree y modifique las reglas solo en OWA (Outlook Web App) hasta que se resuelva el problema.</span><span class="sxs-lookup"><span data-stu-id="c7da2-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="c7da2-111">Si no puede eliminar las reglas manualmente, puede ejecutar un comando de Outlook al iniciar Outlook ejecutando Outlook. exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="c7da2-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="c7da2-112">Se eliminarán las reglas de cliente y de servidor.</span><span class="sxs-lookup"><span data-stu-id="c7da2-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="c7da2-113">Se eliminarán todas las reglas de todas las cuentas del perfil de Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7da2-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="c7da2-114">Este comando se documenta en el artículo modificadores de la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="c7da2-114">This command is further documented in the Command-line switches  article.</span></span>