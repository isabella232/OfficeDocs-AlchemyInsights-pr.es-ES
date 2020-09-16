---
title: Retransmitir correo electrónico a través de Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776503"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a4a99-102">Configurar una aplicación o dispositivo multifunción para enviar correos electrónicos</span><span class="sxs-lookup"><span data-stu-id="a4a99-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a4a99-103">Para obtener más información sobre las opciones disponibles y los pasos, vea [Cómo configurar un dispositivo o aplicación multifunción para enviar correo mediante Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="a4a99-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="a4a99-104">**Nota:** si tiene un dispositivo o aplicación que ha dejado de funcionar recientemente, tenga en cuenta que hemos comenzado a [deshabilitar el cifrado 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) según lo previsto.</span><span class="sxs-lookup"><span data-stu-id="a4a99-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="a4a99-105">Para ver los dispositivos afectados, vaya al [informe de clientes de autenticación SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="a4a99-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="a4a99-106">Los errores comunes podrían ser similares a: error de autenticación, error de TLS, error del algoritmo de cifrado, error de coincidencia del algoritmo o conexión perdida.</span><span class="sxs-lookup"><span data-stu-id="a4a99-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="a4a99-107">Para resolver el problema:</span><span class="sxs-lookup"><span data-stu-id="a4a99-107">To resolve the issue:</span></span>

 - <span data-ttu-id="a4a99-108">**Windows Server 2003 IIS SMTP dejará de funcionar, se necesita una versión más reciente de Windows.**</span><span class="sxs-lookup"><span data-stu-id="a4a99-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="a4a99-109">Póngase en contacto con el proveedor de su aplicación o dispositivo para ver si admite un cifrado moderno o si hay una actualización.</span><span class="sxs-lookup"><span data-stu-id="a4a99-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
