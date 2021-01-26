---
title: El buzón de archivo está casi lleno
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950516"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="ee8d4-102">El buzón de archivo está casi lleno</span><span class="sxs-lookup"><span data-stu-id="ee8d4-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="ee8d4-103">Si el usuario recibe la advertencia; **El buzón de archivo está casi** lleno, o necesita aumentar el tamaño de su buzón de archivo, estas son algunas sugerencias:</span><span class="sxs-lookup"><span data-stu-id="ee8d4-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="ee8d4-104">Si al usuario se le asigna un Plan 1 de Exchange Online, actualice a la licencia del **Plan 2** de Exchange Online para aumentar el tamaño de 50 GB a 100 GB.</span><span class="sxs-lookup"><span data-stu-id="ee8d4-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="ee8d4-105">Si el usuario ya tiene asignada una de las siguientes opciones: **Exchange Online Plan 2** o Exchange Online Plan 1 con un complemento Archivado de Exchange Online, siga estos pasos para habilitar el archivado de expansión automática:.</span><span class="sxs-lookup"><span data-stu-id="ee8d4-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="ee8d4-106">[Conéctese a Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="ee8d4-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="ee8d4-107">Ejecute el siguiente commandlet para el usuario:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="ee8d4-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="ee8d4-108">Ejecute el siguiente commandlet para confirmar que está habilitado para el usuario:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="ee8d4-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="ee8d4-109">Para obtener más información, vea:</span><span class="sxs-lookup"><span data-stu-id="ee8d4-109">For more information see:</span></span>

- [<span data-ttu-id="ee8d4-110"> Habilitar el archivado ilimitado- Ayuda para administradores- Cumplimiento de Microsoft 365 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="ee8d4-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="ee8d4-111">Límites de Exchange Online: descripción del servicio | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="ee8d4-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="ee8d4-112">Actualizar a un plan de negocio | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="ee8d4-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

