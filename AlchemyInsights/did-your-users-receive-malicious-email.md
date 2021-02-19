---
title: ¿Sus usuarios recibieron correo electrónico malicioso?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291809"
---
# <a name="did-your-users-receive-malicious-email"></a>¿Sus usuarios recibieron correo electrónico malicioso?

- Ahora puede notificar el correo electrónico malintencionado a Microsoft de manera sencilla con los [envíos de administración en el Centro de seguridad y cumplimiento](https://sip.protection.office.com/reportsubmission).

Se escanean los mensajes que se envían [envíos de administradores](https://sip.protection.office.com/reportsubmission) y en el control flotante **detalles** se muestran los siguientes resultados:

- Si hubo un error en la autenticación de correo electrónico del remitente en el momento de la entrega.
- Información sobre los aciertos de directiva que puedan haber afectado o invalidado el veredicto de un mensaje.
- Actualice los resultados de cancelación para ver si las direcciones URL o los archivos contenidos en el mensaje son malintencionados o no.
- Comentarios de los calificaciones

Si se encontró una invalidación, se volverá a ejecutar una detección que se completará en unos minutos. Si no había un problema en la autenticación de correo electrónico o si la entrega no se vio afectada por una anulación, los comentarios de los calificadores podrían tardar hasta un día.

Si no está de acuerdo con el veredicto final de un mensaje, dirección URL o archivo (bloqueado frente a no bloqueado), vuelva a enviar el mensaje después de un día para volver a examinarlo. Las probabilidades de que el veredicto cambie después de volver a enviar el mensaje son elevadas.

Mientras tanto, puede quitar el correo electrónico malintencionado de las bandejas de entrada de los usuarios si sigue las instrucciones de [este artículo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Los clientes con Microsoft Defender para Office 365 pueden:
    - usar [Explorador de amenazas para buscar y eliminar correo electrónico sospechoso](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [usar vínculos seguros para bloquear el acceso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a una URL malintencionada
    - realizar un seguimiento de los usuarios que hicieron clic y accedieron a direcciones URL malintencionadas: [Ver URL de suplantación de identidad (phishing) y hacer clic en los datos de veredicto ](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - [Iniciar una investigación automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) de forma manual

También puede protegerse contra archivos y direcciones URL maliciosos con las siguientes instrucciones en [Protección contra archivos y direcciones URL maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).