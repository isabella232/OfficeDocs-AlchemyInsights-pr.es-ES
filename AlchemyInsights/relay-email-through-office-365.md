---
title: Retransmitir correo electrónico a través de Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324379"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurar una aplicación o dispositivo multifunción para enviar correos electrónicos

Para obtener más información sobre las opciones disponibles y los pasos, vea [Cómo configurar un dispositivo o aplicación multifunción para enviar correo mediante Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Si tiene un dispositivo o una aplicación que ha dejado de funcionar recientemente, los problemas más comunes son:

- **Errores relacionados con la autenticación al usar el envío del cliente de autenticación SMTP** Recientemente hemos realizado algunos cambios relacionados con el funcionamiento de la autenticación SMTP. Para obtener más información sobre cómo resolver problemas, vea la sección de autenticación incorrecta de [Corregir problemas con impresoras, escáneres y aplicaciones LOB que envían correo electrónico mediante Microsoft 365 u Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Solo aceptamos la versión 1.2 de TLS al realizar una conexión segura a Office 365** Si usa una Conexión segura (TLS), asegúrese de que el dispositivo de la aplicación admite TLS 1.2. Para obtener más información, consulte [Preparación para TLS 1.2 en Office 365 y Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Para ver otros problemas y soluciones, consulte [Solucionar problemas con impresoras, escáneres y aplicaciones LOB que envían correo electrónico mediante Microsoft 365 u Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Para ver los dispositivos afectados, vaya al [Informe de clientes de autenticación SMTP](https://protection.office.com/mailflow/dashboard).

**Nota**: Exchange Online no admite escenarios de correo masivo. Para enviar correo electrónico comercial masivo (por ejemplo, boletines de clientes) deberían usarse proveedores de terceros especializados en dichos servicios.
