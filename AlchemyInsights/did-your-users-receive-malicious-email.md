---
title: ¿Sus usuarios recibieron correo electrónico malicioso?
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326726"
---
# <a name="did-your-users-receive-malicious-email"></a>¿Sus usuarios recibieron correo electrónico malicioso?

Puede informar a Microsoft del correo electrónico malintencionado utilizando los [Envíos del portal de Microsoft 365 Defender](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Los mensajes que se envían en [envíos de administradores](https://security.microsoft.com/reportsubmission?viewid=admin) se escanean y se muestran los siguientes resultados en el control flotante de detalles:

- Si hubo un error en la autenticación de correo electrónico del remitente en el momento de la entrega.
- Información sobre los aciertos de directiva que puedan haber afectado o invalidado el veredicto de un mensaje.
- Actualice los resultados de cancelación para ver si las direcciones URL o los archivos contenidos en el mensaje son malintencionados o no.
- Comentarios de los calificaciones

Si se ha encontrado un problema de invalidación, el nuevo examen se completará en unos cuantos minutos. Si no existía un problema en la autenticación de correo electrónico o si la entrega no se vio afectada por una invalidación, los comentarios de los calificadores podrían tardar hasta un día.

Si no está de acuerdo con el veredicto final de un mensaje, dirección URL o archivo (bloqueado frente a no bloqueado), vuelva a enviar el mensaje después de un día para volver a examinarlo. Las probabilidades de que el veredicto cambie después de volver a enviar el mensaje son elevadas.

Mientras tanto, puede quitar el correo electrónico malintencionado de las bandejas de entrada de los usuarios si sigue las instrucciones de [este artículo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Los clientes con Microsoft Defender para Office 365 pueden:
  - Usar [Explorador de amenazas para buscar y eliminar correo electrónico sospechoso](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Usar vínculos seguros para bloquear el acceso](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) a una URL malintencionada
  - Realizar un seguimiento de los usuarios que hicieron clic y accedieron a direcciones URL malintencionadas: [Ver URL de suplantación de identidad (phishing) y hacer clic en los datos de veredicto ](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - [Iniciar una investigación automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) de forma manual

También puede protegerse contra archivos y direcciones URL maliciosos con las siguientes instrucciones en [Protección contra archivos y direcciones URL maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
