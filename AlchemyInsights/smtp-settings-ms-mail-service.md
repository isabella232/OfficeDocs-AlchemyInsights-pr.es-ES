---
title: Configuración de SMTP para el servicio de correo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: e4d16a8d04b4d2fb4bfa8cf84308e29f2b499e0680f656cc239411d06e5b077c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900893"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Configuración de SMTP para el servicio de correo Microsoft 365

Esta es la configuración SMTP para los servicios de correo Microsoft 365:

**Servidor**: smtp.office365.com </br>
**Puerto**: 587 </br>
**Cifrado**: STARTTLS (ahora solo se admite la versión TLS 1.2. Asegúrese de que la aplicación o el dispositivo admite TLS 1.2) </br>
**Nombre de usuario**: su dirección de Office 365 (por ejemplo, ejemplo@sudominio.com) </br>
**Contraseña**: su contraseña de Office 365 </br>
**Autenticación**: obligatoria </br>
**Límites de envío**: 10 000 correos electrónicos al día </br>

Para obtener información sobre la configuración de POP e IMAP, consulte [Configuración de POP, IMAP y SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Para obtener más información sobre las opciones para retransmitir correo electrónico mediante Microsoft 365 y los pasos, vea [Cómo configurar un dispositivo o aplicación multifunción para enviar correo mediante Microsoft 365 u Office 365](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).