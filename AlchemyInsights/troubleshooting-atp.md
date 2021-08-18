---
title: Solución de problemas de Microsoft Defender para Office 365
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
ms.openlocfilehash: ea05d60d1cdb4079d52e0a317331f7e98845b82bd74429dc8fa63377c2527a74
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900669"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Solución de problemas de Microsoft Defender para Office 365

- **¿Nota retrasos en la entrega de mensajes?** Usa la [opción Entrega dinámica](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) en tu Microsoft Defender para la directiva Office 365 Caja fuerte datos adjuntos. Esto ayudará a evitar retrasos en los mensajes mientras protege a los destinatarios de archivos malintencionados.

- **¿Desea notificar falsos positivos o falsos negativos a Microsoft?** Use [el Explorador de envíos](https://protection.office.com/reportsubmission).

-** ¿Sabía que puede habilitar la protección de vínculos Caja fuerte para el correo electrónico interno enviado entre destinatarios dentro de su organización?** Siga estos pasos:

  1. Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.

  2. En el panel de navegación izquierdo en **Administración de amenazas,** elija **Directiva** \> **Caja fuerte vínculos**.

  3. En la **sección Directivas que se aplican a toda la organización,** seleccione la directiva y haga clic en **Editar**.

  4. En **Configuración**, habilite **Aplicar vínculos seguros a los mensajes enviados dentro de la organización**.
