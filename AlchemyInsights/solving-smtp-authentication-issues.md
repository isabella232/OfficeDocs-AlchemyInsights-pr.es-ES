---
title: Solucionar problemas de autenticación SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738006"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="f081f-102">Solucionar problemas de autenticación SMTP</span><span class="sxs-lookup"><span data-stu-id="f081f-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="f081f-103">Si recibe los errores 5.7.57 o 5.7.3 al intentar enviar correo electrónico SMTP y autenticarse mediante un cliente o aplicación, puede comprobar algunas cosas:</span><span class="sxs-lookup"><span data-stu-id="f081f-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="f081f-104">Es posible que el envío SMTP autenticado esté deshabilitado en su espacio empresarial o en el buzón que está intentando usar (compruebe ambas configuraciones).</span><span class="sxs-lookup"><span data-stu-id="f081f-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="f081f-105">Para obtener más información, consulte [Habilitar o deshabilitar el envío SMTP de cliente autenticado](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="f081f-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="f081f-106">Compruebe si los [valores predeterminados de seguridad de Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) están habilitados para su espacio empresarial. Si están habilitados, se producirá un error de autenticación SMTP con autenticación básica (también conocido como heredado; este usará el nombre de usuario y la contraseña).</span><span class="sxs-lookup"><span data-stu-id="f081f-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
