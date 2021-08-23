---
title: ¿Le gustaría informar de un falso positivo de correo no deseado a Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396632"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>¿Tiene mensajes legítimos que se marcan como correo no deseado?

Es frustrante cuando un correo electrónico legítimo termina en la carpeta de correo no deseado o en cuarentena. Ten en cuenta estas razones más comunes para los falsos positivos:

**Invalidaciones de inquilinos (más comunes)** Esto está totalmente dentro de su control para corregir.

Enviar el mensaje en Microsoft 365 Defender para analizar las directivas y reglas que afectan; Los detalles de volver a examinar están disponibles en cuestión de minutos.
Revise o modifique las directivas o reglas según corresponda. 

**Invalidaciones de usuario final (comunes)** Esto está totalmente dentro de su control para corregir. 

Enviar el mensaje en Microsoft 365 Defender para analizar las directivas y reglas que afectan; Los detalles de volver a examinar están disponibles en cuestión de minutos. 

Si un mensaje se bloqueó porque se envió desde una dirección de la lista de remitentes bloqueados de un usuario, los encabezados incluyen el veredicto de filtrado de correo no deseado "SFV:BLK".

**Autenticación de correo electrónico de remitentes** Esto está parcialmente dentro del control para corregir.

Enviar el mensaje para analizar errores en la autenticación de correo electrónico del remitente en el momento de la entrega; los resultados están disponibles en un día. 

Si es propietario de la infraestructura de envío, revise cómo alinearla con SPF, DKIM y DMARC para asegurarse de que los sistemas de correo electrónico de destino confían en los mensajes enviados desde su dominio. Como alternativa, póngase en contacto con los remitentes para abordar sus configuraciones dns.

**Veredictos de filtrado de Microsoft** Esto está parcialmente dentro del control para corregir.

Enviar el mensaje e informar del mensaje como seguro; Los resultados de volver a examinar están disponibles en un día. Use la lista de inquilinos permitidos o bloqueados cuando no esté de acuerdo con filtrar veredictos en situaciones concretas. Sin embargo, no debe omitir los veredictos de filtrado de Microsoft de forma permanente. 

Para más información, vea:

- Permitir que los usuarios finales envíen mensajes a Microsoft. Microsoft usa estos envíos para mejorar la eficacia de las tecnologías de protección de correo electrónico y aparecen en los informes de envío para que los use como indicación para actualizar directivas. 

- Para ver un breve vídeo sobre el envío de mensajes para su análisis, consulte [Submitting messages for analysis](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Usar el Envío para administradores para enviar correo no deseado, de suplantación de identidad, direcciones URL y archivos sospechosos a Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Administrar la lista de bloqueados y permitidos del espacio empresarial](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Encabezados de mensajes de correo no deseado en Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Protección contra correo no deseado saliente en EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)