---
title: Solucionar problemas de autenticación SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826432"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="07602-102">Solucionar problemas de autenticación SMTP</span><span class="sxs-lookup"><span data-stu-id="07602-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="07602-103">Si recibe los errores 5.7.57 o 5.7.3 al intentar enviar correo electrónico SMTP y autenticarse mediante un cliente o aplicación, puede comprobar algunas cosas:</span><span class="sxs-lookup"><span data-stu-id="07602-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="07602-104">Es posible que el envío SMTP autenticado esté deshabilitado en su espacio empresarial o en el buzón que está intentando usar (compruebe ambas configuraciones).</span><span class="sxs-lookup"><span data-stu-id="07602-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="07602-105">Para obtener más información, consulte [Habilitar o deshabilitar el envío SMTP de cliente autenticado](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="07602-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="07602-106">Compruebe si los [valores predeterminados de seguridad de Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) están habilitados para su espacio empresarial. Si están habilitados, se producirá un error de autenticación SMTP con autenticación básica (también conocido como heredado; este usará el nombre de usuario y la contraseña).</span><span class="sxs-lookup"><span data-stu-id="07602-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
