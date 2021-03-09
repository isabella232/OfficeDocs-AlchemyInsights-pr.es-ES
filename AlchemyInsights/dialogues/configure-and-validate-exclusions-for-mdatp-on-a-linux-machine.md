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
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>Configurar y validar exclusiones para MDATP en una máquina Linux

Puede excluir determinados archivos, carpetas, procesos y archivos abiertos por procesos de los exámenes MDATP. Las exclusiones ayudan a evitar la detección incorrecta de software y archivos únicos o personalizados para su organización. Las exclusiones también ayudan a mitigar los problemas de rendimiento causados por MDATP.

Para obtener más información, vea [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).

> [!IMPORTANT]
> Las exclusiones descritas en este artículo no se aplican a otras funcionalidades de MDATP para Linux, incluida la detección y respuesta de puntos de conexión (EDR). Los archivos que se excluyen mediante los métodos descritos en este artículo aún pueden desencadenar alertas de EDR y otras funcionalidades de detección.
