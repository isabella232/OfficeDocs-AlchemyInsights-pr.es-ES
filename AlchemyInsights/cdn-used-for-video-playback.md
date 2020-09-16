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
# <a name="cdn-used-for-video-playback"></a>CDN que se usa para la reproducción de vídeo

Los eventos en directo de Stream y los eventos en directo de aplicaciones o dispositivos externos de Yammer/Teams usarán automáticamente la red Azure CDN. Los vídeos a petición cargados en Stream aún no usan Azure CDN para la reproducción. Los vídeos en diferido de Stream se reproducen desde el servidor de origen de Azure Media Services asociado al inquilino en la región geográfica del inquilino. Para obtener más información, vea:

- [Red CDN utilizada para la reproducción de vídeo](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
