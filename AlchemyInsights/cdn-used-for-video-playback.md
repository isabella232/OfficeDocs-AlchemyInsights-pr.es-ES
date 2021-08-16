---
title: CDN que se usa para la reproducción de vídeo
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
- "9002552"
- "5146"
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071133"
---
# <a name="cdn-used-for-video-playback"></a>CDN que se usa para la reproducción de vídeo

Los eventos en directo de Stream y los eventos en directo de aplicaciones o dispositivos externos de Yammer/Teams usarán automáticamente la red Azure CDN. Los vídeos a petición cargados en Stream aún no usan Azure CDN para la reproducción. Los vídeos en diferido de Stream se reproducen desde el servidor de origen de Azure Media Services asociado al inquilino en la región geográfica del inquilino. Para obtener más información, vea:

- [Red CDN utilizada para la reproducción de vídeo](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
