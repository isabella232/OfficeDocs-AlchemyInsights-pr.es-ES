---
title: Problemas de rendimiento en Microsoft Defender para punto de conexión en Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783444"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="41a07-102">Problemas de rendimiento en Microsoft Defender para punto de conexión en Linux</span><span class="sxs-lookup"><span data-stu-id="41a07-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="41a07-103">Este artículo le mostrará los pasos para identificar problemas de rendimiento en Microsoft Defender para punto de conexión en Linux.</span><span class="sxs-lookup"><span data-stu-id="41a07-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="41a07-104">Es importante que primero compruebe si el problema que experimenta se ha resuelto en la[última versión](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="41a07-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="41a07-105">Para iniciar su investigación, consulte cómo [Resolver problemas de rendimiento de Microsoft Defender para punto de conexión para Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="41a07-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="41a07-106">Exclusiones</span><span class="sxs-lookup"><span data-stu-id="41a07-106">Exclusions</span></span>

<span data-ttu-id="41a07-107">Las exclusiones pueden ayudar a mitigar los problemas de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="41a07-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="41a07-108">Revise las exclusiones antes de empezar para que se conozca y documente cualquier riesgo adicional.</span><span class="sxs-lookup"><span data-stu-id="41a07-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="41a07-109">Para más información, consulte [Configurar y validar exclusiones de Microsoft Defender para punto de conexión en Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="41a07-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="41a07-110">Si tiene varios archivos y carpetas a excluir y están todos en el mismo punto de montaje, puede ser más fácil excluir el punto de montaje.</span><span class="sxs-lookup"><span data-stu-id="41a07-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="41a07-111">A partir de la versión 101.22.80 de febrero, se permite excluir un punto de montaje entero.</span><span class="sxs-lookup"><span data-stu-id="41a07-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="41a07-112">Por ejemplo, si /mnt/backup es un punto de montaje, puede agregar /mnt/backup a la lista de exclusión con este comando:</span><span class="sxs-lookup"><span data-stu-id="41a07-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="41a07-113">**Nota**: Agregar exclusiones aumenta el riesgo de que no se detecte malware y debe administrarse e implementarse con cuidado.</span><span class="sxs-lookup"><span data-stu-id="41a07-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="41a07-114">¿Necesita ayuda?</span><span class="sxs-lookup"><span data-stu-id="41a07-114">Need Help?</span></span>

<span data-ttu-id="41a07-115">Para ayudarle de la manera más eficaz, recopile los datos de diagnóstico antes de abrir un caso de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="41a07-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
