---
title: Cifrado con reglas de transporte
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813885"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="472db-102">Cifrado con reglas de transporte</span><span class="sxs-lookup"><span data-stu-id="472db-102">Encryption with transport rules</span></span>

<span data-ttu-id="472db-103">En el [Centro de administración de Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), puede usar las funciones de cifrado de mensajes de Office (OME) en las reglas de flujo del correo para desencadenar el cifrado de mensajes.</span><span class="sxs-lookup"><span data-stu-id="472db-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="472db-104">Elija la opción **Aplicar el cifrado de mensajes de Office 365 y la protección de derechos** en la condición de Regla de transporte.</span><span class="sxs-lookup"><span data-stu-id="472db-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="472db-105">Para más información, consulte [Definir regla de flujo de correo para cifrar](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="472db-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="472db-106">En PowerShell, use el cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) y establezca el parámetro *ApplyOME* en $true.</span><span class="sxs-lookup"><span data-stu-id="472db-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
