---
title: Solucionar problemas de instalación de MDATP en un Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737660"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Solucionar problemas de instalación de MDATP en un Mac

Si se produce un error en la instalación manual, la página **Resumen** del asistente para la instalación muestra el siguiente error:

"Se ha producido un error durante la instalación. El instalador encontró un error que provocó un error en la instalación. Póngase en contacto con el fabricante del software para obtener ayuda."

Para las implementaciones de MDM, la página también muestra un error de instalación genérica.

Aunque no mostremos errores exactos a los usuarios finales, guardamos un archivo de registro con el progreso de la instalación, en **/Library/Logs/Microsoft/mdatp/install.log**. Cada sesión de instalación se anexa a este archivo de registro. Para generar solo la última sesión de instalación, use `sed` .

Para obtener más información, vea [Solucionar problemas de instalación de ATP de Microsoft Defender para Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
