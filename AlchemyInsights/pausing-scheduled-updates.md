---
title: Pausar actualizaciones programadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530597"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="0af4a-102">Pausar actualizaciones programadas</span><span class="sxs-lookup"><span data-stu-id="0af4a-102">Pausing scheduled updates</span></span>

<span data-ttu-id="0af4a-103">Cuando se ejecuta un comando pause, los dispositivos no procesan el comando hasta la próxima vez que se registran en Intune.</span><span class="sxs-lookup"><span data-stu-id="0af4a-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="0af4a-104">Por este motivo, es posible que los dispositivos:</span><span class="sxs-lookup"><span data-stu-id="0af4a-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="0af4a-105">Tengan instaladas las actualizaciones programadas antes del registro.</span><span class="sxs-lookup"><span data-stu-id="0af4a-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="0af4a-106">Se hayan apagado cuando se emitió el comando pause.</span><span class="sxs-lookup"><span data-stu-id="0af4a-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="0af4a-107">En este caso, cuando se enciendan los dispositivos, es posible que se hayan descargado e instalado las actualizaciones programadas anteriores al registro.</span><span class="sxs-lookup"><span data-stu-id="0af4a-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>