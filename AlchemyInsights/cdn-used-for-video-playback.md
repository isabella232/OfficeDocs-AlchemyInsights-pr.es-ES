---
title: CDN que se usa para la reproducción de vídeo
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
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756984"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="3856f-102">CDN que se usa para la reproducción de vídeo</span><span class="sxs-lookup"><span data-stu-id="3856f-102">CDN used for video playback</span></span>

<span data-ttu-id="3856f-103">Los eventos en directo de Stream y los eventos en directo de aplicaciones o dispositivos externos de Yammer/Teams usarán automáticamente la red Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="3856f-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="3856f-104">Los vídeos a petición cargados en Stream aún no usan Azure CDN para la reproducción.</span><span class="sxs-lookup"><span data-stu-id="3856f-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="3856f-105">Los vídeos en diferido de Stream se reproducen desde el servidor de origen de Azure Media Services asociado al inquilino en la región geográfica del inquilino.</span><span class="sxs-lookup"><span data-stu-id="3856f-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="3856f-106">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="3856f-106">For more information, see:</span></span>

- [<span data-ttu-id="3856f-107">Red CDN utilizada para la reproducción de vídeo</span><span class="sxs-lookup"><span data-stu-id="3856f-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
