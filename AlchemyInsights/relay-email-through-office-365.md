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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118000"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="bc83a-102">Configurar una aplicación o dispositivo multifunción para enviar correos electrónicos</span><span class="sxs-lookup"><span data-stu-id="bc83a-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="bc83a-103">Para obtener más información sobre las opciones disponibles y los pasos, vea [Cómo configurar un dispositivo o aplicación multifunción para enviar correo mediante Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="bc83a-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="bc83a-104">Si tiene un dispositivo o una aplicación que ha dejado de funcionar recientemente, los problemas más comunes son:</span><span class="sxs-lookup"><span data-stu-id="bc83a-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="bc83a-105">**Errores relacionados con la autenticación al usar el envío del cliente de autenticación SMTP** Recientemente hemos realizado algunos cambios relacionados con el funcionamiento de la autenticación SMTP.</span><span class="sxs-lookup"><span data-stu-id="bc83a-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="bc83a-106">Para obtener más información sobre cómo resolver problemas, vea la sección de autenticación incorrecta de [Corregir problemas con impresoras, escáneres y aplicaciones LOB que envían correo electrónico mediante Microsoft 365 u Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="bc83a-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="bc83a-107">**Solo aceptamos la versión 1.2 de TLS al realizar una conexión segura a Office 365** Si usa una Conexión segura (TLS), asegúrese de que el dispositivo de la aplicación admite TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="bc83a-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="bc83a-108">Para obtener más información, consulte [Preparación para TLS 1.2 en Office 365 y Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="bc83a-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="bc83a-109">Para ver otros problemas y soluciones, consulte [Solucionar problemas con impresoras, escáneres y aplicaciones LOB que envían correo electrónico mediante Microsoft 365 u Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span><span class="sxs-lookup"><span data-stu-id="bc83a-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="bc83a-110">Para ver los dispositivos afectados, vaya al [Informe de clientes de autenticación SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="bc83a-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="bc83a-p103">**Nota**: Exchange Online no admite escenarios de correo masivo. Para enviar correo electrónico comercial masivo (por ejemplo, boletines de clientes) deberían usarse proveedores de terceros especializados en dichos servicios.</span><span class="sxs-lookup"><span data-stu-id="bc83a-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
