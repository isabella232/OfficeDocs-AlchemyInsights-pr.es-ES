---
title: Habilitar la auditoría de buzones de correo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806308"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="ec2da-102">Habilitar la auditoría de buzones de correo</span><span class="sxs-lookup"><span data-stu-id="ec2da-102">Enable mailbox auditing</span></span>

<span data-ttu-id="ec2da-103">Para habilitar la auditoría de buzones de correo para un solo usuario o para toda una organización, los siguientes cmdlets deben ejecutarse desde el shell de alimentación remota:</span><span class="sxs-lookup"><span data-stu-id="ec2da-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="ec2da-104">**Usuario único**</span><span class="sxs-lookup"><span data-stu-id="ec2da-104">**Single User**</span></span>
  
<span data-ttu-id="ec2da-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="ec2da-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="ec2da-106">**Organización**</span><span class="sxs-lookup"><span data-stu-id="ec2da-106">**Organization**</span></span>
  
<span data-ttu-id="ec2da-107">Get-Mailbox-Resultsize-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="ec2da-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="ec2da-108">Más información</span><span class="sxs-lookup"><span data-stu-id="ec2da-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

