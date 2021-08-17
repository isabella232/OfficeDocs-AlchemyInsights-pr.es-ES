---
title: Solución de problemas cuando un trabajo del Servicio de importación se bloquea
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105117"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Solución de problemas cuando un trabajo del Servicio de importación se bloquea

Si tiene problemas con trabajos del Servicio de importación que se bloquean o tienen errores, consulte y pruebe lo siguiente:

- Revise el tamaño del archivo PST. El tamaño máximo recomendado para importar un archivo PST es de 20 GB.

- Si sospecha que se omitieron elementos debido a daños, ejecute Scanpst.exe para diagnosticar y corregir errores en los archivos PST.

- Si ve el error "MapiExceptionShutoffQuotaExceeded" durante la importación, asegúrese de que el buzón de destino tenga capacidad suficiente para importar los archivos PST deseados.

Para más información sobre cómo solucionar problemas relacionados con trabajos de importación de PST, consulte [Solución de problemas relacionados con trabajos de importación de PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Para obtener información sobre cómo corregir problemas al importar PST en Outlook, consulte [Solucionar problemas al importar un archivo .pst de Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).