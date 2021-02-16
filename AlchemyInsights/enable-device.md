---
title: Habilitar dispositivo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255182"
---
# <a name="enable-device"></a>Habilitar dispositivo

**Para habilitar el dispositivo mediante el comando de PowerShell**

Ejecute los comandos siguientes:

- Para obtener el objeto device: `Get-MsolDevice -Name <Name>`
- Para habilitar el dispositivo: `Enable-MsolDevice -DeviceId <DeviceId>`

Para obtener más información sobre cómo configurar la unión híbrida en dominios administrados, vea [Configurar la unión híbrida.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
