---
title: Solucionar los errores de retención de eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1ce8443549ea111bc3ebba9c30c4e621a04926231c24d34c64b6d024194d5249
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886272"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Solucionar los errores de retención de eDiscovery

¿Está teniendo problemas con las retenciones de eDiscovery? Estos son algunos procedimientos recomendados que puede probar:

- Compruebe el estado de distribución de retención.  Si el estado es **Activado (pendiente)** o **Desactivado (pendiente)**, espere a que se complete la distribución de la retención.
- Combine las actualizaciones de retención de eDiscovery en una sola solicitud en masa en lugar de actualizar la directiva repetidamente para cada transacción.
- Ejecute Set-CaseHoldPolicy <policyname> -RetryDistribution en el Powershell del Centro de seguridad y cumplimiento. Para más información, consulte [Conectarse al PowerShell del Centro de seguridad y cumplimiento](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell).

Para ver los pasos para comprobar esta configuración y los procedimientos recomendados adicionales para mitigar y resolver problemas de retención de eDiscovery, vea [Solucionar problemas de retención de eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors).
Para obtener información sobre cómo solucionar otros problemas comunes de eDiscovery, consulte [Investigar y solucionar comunes de eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
