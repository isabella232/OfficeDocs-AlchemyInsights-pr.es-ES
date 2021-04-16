---
title: 'Problema de activación: no podemos conectarnos en este momento'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806459"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Corregir el mensaje de aplicaciones de Microsoft 365 "No podemos conectarnos en este momento"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a las aplicaciones de Microsoft 365. Consulte [Direcciones URL de Microsoft e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vaya a **Iniciar**  >  **ejecución** y, a continuación, escriba **services.msc**. Asegúrese de que todos los servicios siguientes están en ejecución:
    - Configuración automática de dispositivos conectados en red
    - Servicio de lista de red
    - Reconocimiento de ubicación de red
    - Registro de eventos de Windows

Si uno de estos servicios no se está ejecutando, intente iniciarlo. Si tiene un problema al iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:

**sfc /scannow**

Cuando finalice este comando, reinicie el equipo.

Para obtener información detallada, consulta ["Lo sentimos, no podemos conectarnos a tu cuenta. Vuelva a intentarlo más adelante" error al activar Office desde Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).