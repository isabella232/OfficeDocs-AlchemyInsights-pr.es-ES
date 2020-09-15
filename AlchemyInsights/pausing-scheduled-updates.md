---
title: Pausar actualizaciones programadas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721572"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="b6bb7-102">Pausar actualizaciones programadas</span><span class="sxs-lookup"><span data-stu-id="b6bb7-102">Pausing scheduled updates</span></span>

<span data-ttu-id="b6bb7-103">Cuando se ejecuta un comando pause, los dispositivos no procesan el comando hasta la próxima vez que se registran en Intune.</span><span class="sxs-lookup"><span data-stu-id="b6bb7-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="b6bb7-104">Por este motivo, es posible que los dispositivos:</span><span class="sxs-lookup"><span data-stu-id="b6bb7-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="b6bb7-105">Tengan instaladas las actualizaciones programadas antes del registro.</span><span class="sxs-lookup"><span data-stu-id="b6bb7-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="b6bb7-106">Se hayan apagado cuando se emitió el comando pause.</span><span class="sxs-lookup"><span data-stu-id="b6bb7-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="b6bb7-107">En este caso, cuando se enciendan los dispositivos, es posible que se hayan descargado e instalado las actualizaciones programadas anteriores al registro.</span><span class="sxs-lookup"><span data-stu-id="b6bb7-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>