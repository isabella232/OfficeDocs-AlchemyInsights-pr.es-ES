---
title: Corregir reglas de transporte
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568681"
---
# <a name="fix-transport-rules"></a>Corregir reglas de transporte

Una regla de flujo de correo personalizada afectó a este mensaje. Para revisar la regla exacta, haga lo siguiente:

1. En los resultados de envío, en **Información adicional**, anote el **GUID** o el nombre de **la directiva**.
2. Inicie el Shell de administración de Exchange. Para obtener más información, vea [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Ejecute este comando (mediante el GUID del envío):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Revise la descripción para ver las condiciones configuradas que afectaron al mensaje.

Para obtener más información, [vea Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
