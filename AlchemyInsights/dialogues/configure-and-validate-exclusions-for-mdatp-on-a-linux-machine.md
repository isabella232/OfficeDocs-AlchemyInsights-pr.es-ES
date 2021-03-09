---
title: Configurar y validar exclusiones para MDATP en una máquina Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568717"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="3b639-102">Configurar y validar exclusiones para MDATP en una máquina Linux</span><span class="sxs-lookup"><span data-stu-id="3b639-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="3b639-103">Puede excluir determinados archivos, carpetas, procesos y archivos abiertos por procesos de los exámenes MDATP.</span><span class="sxs-lookup"><span data-stu-id="3b639-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="3b639-104">Las exclusiones ayudan a evitar la detección incorrecta de software y archivos únicos o personalizados para su organización.</span><span class="sxs-lookup"><span data-stu-id="3b639-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="3b639-105">Las exclusiones también ayudan a mitigar los problemas de rendimiento causados por MDATP.</span><span class="sxs-lookup"><span data-stu-id="3b639-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="3b639-106">Para obtener más información, vea [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="3b639-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3b639-107">Las exclusiones descritas en este artículo no se aplican a otras funcionalidades de MDATP para Linux, incluida la detección y respuesta de puntos de conexión (EDR).</span><span class="sxs-lookup"><span data-stu-id="3b639-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="3b639-108">Los archivos que se excluyen mediante los métodos descritos en este artículo aún pueden desencadenar alertas de EDR y otras funcionalidades de detección.</span><span class="sxs-lookup"><span data-stu-id="3b639-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
