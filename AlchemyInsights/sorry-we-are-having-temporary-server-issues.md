---
title: Corregir Microsoft 365 aplicaciones Lo sentimos, tenemos un mensaje de problemas temporales de servidor
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
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021613"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Corregir el mensaje Microsoft 365 "Lo sentimos, estamos teniendo problemas temporales de servidor"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a Microsoft 365 aplicaciones. Consulte [DIRECCIONES URL e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vaya a **Iniciar**  >  **ejecución** y, a continuación, escriba **services.msc**. Asegúrese de que todos los servicios siguientes están en ejecución:
    - Configuración automática de dispositivos conectados en red
    - Servicio de lista de red
    - Reconocimiento de ubicación de red
    - Registro de eventos de Windows

Si uno de estos servicios no se está ejecutando, intente iniciarlo. Si tiene un problema al iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:

**sfc /scannow**

Cuando finalice este comando, reinicie el equipo.

Para obtener información detallada, consulta ["Lo sentimos, no podemos conectarnos a tu cuenta. Vuelva a intentarlo más adelante" error al activar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).