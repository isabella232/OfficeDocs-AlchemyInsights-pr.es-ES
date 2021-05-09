---
title: ¿Necesita marcar un dominio o remitente de correo electrónico como seguro?
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
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286697"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>¿Necesita marcar un dominio o remitente de correo electrónico como seguro?

- No se recomienda el uso de **listas de remitentes seguros** ya que expone su organización a ataques de spam, phishing y suplantación de identidad.
- Sin embargo, si hay un requisito empresarial, **recomendamos** usar **[Reglas de flujo de correo](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** para esto. Nuestra guía garantiza la autenticación del remitente (comprueba que el dominio remitente no está falsificado). **Nota**: no recomendamos administrar los falsos positivos con las listas de remitentes seguros, ya que las excepciones al filtrado de correo no deseado pueden exponer la organización a ataques de seguridad. Si los usuarios reciben mensajes que se marcan incorrectamente como spam o correo electrónico no deseado, puede **[Informar de los mensajes y archivos a Microsoft](https://protection.office.com/reportsubmission)**.
- **Deberían evitarse** los remitentes seguros en Outlook, la lista de remitentes permitidos o la lista de dominios permitidos en las directivas antispam porque los remitentes omiten toda la protección contra correo no deseado, suplantación de identidad, protección contra phishing y autenticación de remitente (SPF, DKIM, DMARC). Este método es más adecuado solo para las pruebas temporales.
- La validación de que un correo electrónico determinado ha omitido la evaluación de correo no deseado puede realizarse mediante la comprobación del encabezado de mensaje "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), vea **[Encabezados de mensaje de correo no deseado](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Como Microsoft quiere [proteger de forma predeterminada](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions) a nuestros clientes, no se aplican ciertas invalidaciones de espacio empresarial para el malware y la suplantación de identidad (phishing) de alta confianza. Estas invalidaciones incluyen: o   Listas de remitentes permitidos o listas de dominios permitidos (directivas contra correo no deseado) o   Remitentes seguros de Outlook o   Lista de permitidos de IP (filtrado de conexión) 
- La única invalidación que permite que el mensaje de suplantación de identidad (phishing) de alta confianza omita el filtrado son las reglas de flujo de correo de Exchange (también conocidas como reglas de transporte). Para usar reglas de flujo de correo para omitir el filtrado, vea **[Usar reglas de flujo de correo para establecer el nivel de confianza contra correo no deseado (SCL) en los mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.