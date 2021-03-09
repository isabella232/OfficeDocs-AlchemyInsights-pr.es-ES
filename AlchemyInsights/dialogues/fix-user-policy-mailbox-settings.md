---
title: Corregir la configuración de la directiva de usuario/buzón de correo
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568688"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="376cc-102">Corregir la configuración de la directiva de usuario/buzón de correo</span><span class="sxs-lookup"><span data-stu-id="376cc-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="376cc-103">La configuración del correo no deseado en el buzón afectó a este mensaje.</span><span class="sxs-lookup"><span data-stu-id="376cc-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="376cc-104">Para revisar la configuración, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="376cc-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="376cc-105">Inicie el Shell de administración de Exchange.</span><span class="sxs-lookup"><span data-stu-id="376cc-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="376cc-106">Para obtener más información, vea [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="376cc-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="376cc-107">Ejecute este comando (mediante la dirección de correo electrónico del usuario):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="376cc-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="376cc-108">Compruebe si la dirección de correo electrónico del remitente forma parte de **TrustedSendersAndDomains** o **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="376cc-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="376cc-109">Si la dirección de correo electrónico está en una de las listas, es posible que tenga que quitarla.</span><span class="sxs-lookup"><span data-stu-id="376cc-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="376cc-110">Para obtener más información, [vea Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="376cc-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
