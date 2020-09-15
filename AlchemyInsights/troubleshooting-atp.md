---
title: Solución de problemas de la protección contra amenazas avanzada de Office 365
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658931"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a>Solución de problemas de la protección contra amenazas avanzada de Office 365

- ¿Observa retrasos en la entrega de mensajes? Use la opción de [entrega dinámica](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) en la Directiva de datos adjuntos seguros de ATP. Esto ayudará a evitar los retrasos en los mensajes al proteger a los destinatarios de archivos malintencionados.

- ¿Desea informar de falsos positivos o falsos negativos a Microsoft? Use este [vínculo](https://www.microsoft.com/wdsi/filesubmission/) para enviar archivos para su análisis.

- ¿Sabía que puede habilitar la protección de vínculos seguros para el correo electrónico interno que se envía entre los destinatarios de la organización? Siga estos pasos:

  1. Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.

  2. En el panel de navegación izquierdo, en **Administración de amenazas**, elija **Policy** \> **vínculos seguros**de directiva.

  3. En la sección **directivas que se aplican a toda la organización** , seleccione la Directiva y haga clic en **Editar**.

  4. En **configuración**, habilite **aplicar vínculos seguros a los mensajes enviados dentro de la organización**.
