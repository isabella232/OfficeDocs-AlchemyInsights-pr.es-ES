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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998189"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Corregir el Microsoft 365 de aplicaciones "No podemos conectarnos en este momento"

Si recibe este mensaje, pruebe lo siguiente:

1. Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a Microsoft 365 aplicaciones. Consulte [Direcciones URL de Microsoft e intervalos de direcciones IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Vaya a **Iniciar**  >  **ejecución** y, a continuación, escriba **services.msc**. Asegúrese de que todos los servicios siguientes están en ejecución:
    - Configuración automática de dispositivos conectados en red
    - Servicio de lista de red
    - Reconocimiento de ubicación de red
    - Registro de eventos de Windows

Si uno de estos servicios no se está ejecutando, intente iniciarlo. Si tiene un problema al iniciar el servicio, ejecute el siguiente comando abriendo un símbolo del sistema con permisos elevados:

**sfc /scannow**

Cuando finalice este comando, reinicie el equipo.

Para obtener información detallada, consulta ["Lo sentimos, no podemos conectarnos a tu cuenta. Vuelva a intentarlo más adelante" error](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)al activar Office desde Microsoft 365 .