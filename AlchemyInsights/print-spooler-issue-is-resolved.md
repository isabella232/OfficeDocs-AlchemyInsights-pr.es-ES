---
title: Se ha resuelto el problema con el administrador de trabajos de impresión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911355"
---
# <a name="print-spooler-issue-is-resolved"></a>Se ha resuelto el problema con el administrador de trabajos de impresión

Si su dispositivo se ha actualizado con la **compilación de sistema operativo 19041.329** de Windows 10, es posible que haya observado un fallo de impresión en ciertas impresoras. Puede que el administrador de trabajos de impresión indique un error o que se cierre de manera inesperada al intentar imprimir y que la impresora afectada no produzca ningún resultado. Este problema se resuelve en la compilación de sistema operativo **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Investigación en curso**

Es posible que el archivo del Servicio de subsistema de autoridad de seguridad local, o LSASS (**Isass.exe**), produzca errores en algunos dispositivos y genere el siguiente mensaje de error: "Un proceso crítico del sistema, C:\WINDOWS\system32\Isass.exe, ha producido un error con el código de estado c0000008. Es necesario reiniciar el equipo ahora".  **Microsoft está trabajando en una solución y le ofrecerá una actualización en una versión futura.**

Para más información, consulte los [problemas conocidos de la versión 2004 de Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).