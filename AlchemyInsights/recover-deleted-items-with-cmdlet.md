---
title: Recuperar elementos eliminados con un cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741320"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="c07df-102">Recuperar elementos eliminados con un cmdlet</span><span class="sxs-lookup"><span data-stu-id="c07df-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="c07df-103">Use el cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) para ver los elementos eliminados en los buzones.</span><span class="sxs-lookup"><span data-stu-id="c07df-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="c07df-104">Cuando encuentre los elementos eliminados, use el cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) para restaurarlos.</span><span class="sxs-lookup"><span data-stu-id="c07df-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="c07df-105">Vea todos los detalles de [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c07df-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="c07df-106">Debe tener asignado el rol de exportación e importación de buzón de correo antes de que pueda ejecutar este cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c07df-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="c07df-107">Para obtener más información, consulte [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="c07df-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
