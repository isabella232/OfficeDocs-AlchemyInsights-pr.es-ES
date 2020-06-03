---
title: Solución de problemas con la protección contra amenazas avanzada de Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511129"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Solucionar problemas con Office 365 ATP

- ¿Hay **retrasos en la entrega de mensajes de correo electrónico**? Pruebe a usar la opción de entrega dinámica para las directivas de datos adjuntos seguros de ATP. Esto evitará los retrasos en la entrega de mensajes de correo electrónico al proteger a los destinatarios de archivos malintencionados.
- **¿Desea informar de falsos positivos o falsos negativos**? Use este vínculo para enviar el archivo para su análisis:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **¿Sabía que puede habilitar la protección de vínculos seguros de ATP para el correo electrónico que se envía entre las personas de su organización**? Siga estos pasos:
    1. Vaya a https://protection.office.com e inicie sesión.
    2. Vaya a **Threat management**  >  **Policy**  >  **vínculos seguros**de la Directiva de administración de amenazas.
    3. En **directivas que se aplican a destinatarios específicos**, edite (o agregue) una directiva.
    4. Seleccione **aplicar vínculos seguros a los mensajes enviados dentro de la organización**.
    5. Guarde la Directiva y espere unos 30 minutos para que los cambios funcionen en el centro de proceso de información.
- Para obtener más ayuda con ATP, consulte [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).