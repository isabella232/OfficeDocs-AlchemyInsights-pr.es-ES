---
title: Corregir aplicaciones de Microsoft 365 Lo sentimos, tenemos un mensaje de problemas temporales de servidor
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835288"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corregir el mensaje de aplicaciones de Microsoft 365 "Lo sentimos, estamos teniendo problemas temporales de servidor"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a las aplicaciones de Microsoft 365. Consulte [DIRECCIONES URL e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vaya a **Iniciar**  >  **ejecución** y, a continuación, escriba **services.msc**. Asegúrese de que todos los servicios siguientes están en ejecución:
    - Configuración automática de dispositivos conectados en red
    - Servicio de lista de red
    - Reconocimiento de ubicación de red
    - Registro de eventos de Windows

Si uno de estos servicios no se está ejecutando, intente iniciarlo. Si tiene un problema al iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:

**sfc /scannow**

Cuando finalice este comando, reinicie el equipo.

Para obtener información detallada, consulta ["Lo sentimos, no podemos conectarnos a tu cuenta. Vuelva a intentarlo más adelante" error al activar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).