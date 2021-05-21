---
title: Complemento de Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582087"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="97abe-102">Complemento de Teams para Mac</span><span class="sxs-lookup"><span data-stu-id="97abe-102">Teams add-in for Mac</span></span>

<span data-ttu-id="97abe-103">Para solucionar la falta de un complemento de Teams para los usuarios del sistema operativo Mac, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="97abe-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="97abe-104">**Paso 1:** si tiene una implementación local de Exchange híbrida (2016 CU3 o posterior requerido), use la herramienta Test-HMA.ps1 para confirmar que la autenticación moderna híbrida está configurada correctamente.</span><span class="sxs-lookup"><span data-stu-id="97abe-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="97abe-105">Para más información, consulte [Validar la configuración de la autenticación moderna híbrida para Outlook para iOS y Android](https://aka.ms/TestHMAEAS).</span><span class="sxs-lookup"><span data-stu-id="97abe-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="97abe-106">**Nota:** utilice el formato de dirección UPN (por ejemplo, [username@contoso.com](mailto:username@contoso.com)), no el formato dominio\nombre de usuario.</span><span class="sxs-lookup"><span data-stu-id="97abe-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="97abe-107">Haga esto incluso para los usuarios con buzones de Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="97abe-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="97abe-108">**Paso 2:** haga que el usuario vaya a **Herramientas** > **Cuentas**... en Outlook para Mac y busque y seleccione la cuenta.</span><span class="sxs-lookup"><span data-stu-id="97abe-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="97abe-109">Confirme que el nombre de usuario que aparece en la lista está en formato UPN (por ejemplo, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="97abe-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="97abe-110">**Paso 3:** confirme que el usuario tiene licencia de Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="97abe-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="97abe-111">El usuario debe usar la suscripción a Office 365 para Mac, versión del producto 16.24 o posterior.</span><span class="sxs-lookup"><span data-stu-id="97abe-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>