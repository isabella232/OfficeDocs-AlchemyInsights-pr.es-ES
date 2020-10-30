---
title: Solución de problemas de Microsoft defender para Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801463"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Solución de problemas de Microsoft defender para Office 365

- ¿Observa retrasos en la entrega de mensajes? Use la opción de [entrega dinámica](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) en la Directiva de datos adjuntos seguros de ATP. Esto ayudará a evitar los retrasos en los mensajes al proteger a los destinatarios de archivos malintencionados.

- ¿Desea informar de falsos positivos o falsos negativos a Microsoft? Use este [vínculo](https://www.microsoft.com/wdsi/filesubmission/) para enviar archivos para su análisis.

- ¿Sabía que puede habilitar la protección de vínculos seguros para el correo electrónico interno que se envía entre los destinatarios de la organización? Siga estos pasos:

  1. Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.

  2. En el panel de navegación izquierdo, en **Administración de amenazas** , elija **Policy** \> **vínculos seguros** de directiva.

  3. En la sección **directivas que se aplican a toda la organización** , seleccione la Directiva y haga clic en **Editar** .

  4. En **configuración** , habilite **aplicar vínculos seguros a los mensajes enviados dentro de la organización** .
