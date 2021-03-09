---
title: Error de dirección proxy al crear un buzón compartido
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568307"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="c3d18-102">Error de dirección de proxy al crear un buzón u otro objeto habilitado para correo electrónico</span><span class="sxs-lookup"><span data-stu-id="c3d18-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="c3d18-103">Si intentó crear un objeto habilitado para correo electrónico (buzón de correo, buzón compartido, etc.) y recibió el error "La dirección proxy "SMTP:alias@domain.com" ya se está utilizando...", la dirección de correo electrónico que eligió ya la toma otro objeto habilitado para correo electrónico de su organización.</span><span class="sxs-lookup"><span data-stu-id="c3d18-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="c3d18-104">Debe buscar el usuario, grupo, buzón compartido o carpeta pública que tiene esta dirección de correo electrónico y eliminarlo o cambiar su dirección de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="c3d18-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="c3d18-105">A continuación, puede crear un nuevo objeto habilitado para correo electrónico con la dirección de correo electrónico liberada.</span><span class="sxs-lookup"><span data-stu-id="c3d18-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="c3d18-106">Use La búsqueda en la página principal para encontrarlo.</span><span class="sxs-lookup"><span data-stu-id="c3d18-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="c3d18-107">También puede usar el siguiente comando de PowerShell de Exchange Online para buscarlo:</span><span class="sxs-lookup"><span data-stu-id="c3d18-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="c3d18-108">Si no desea eliminar la dirección de correo electrónico existente, elija una nueva dirección de correo electrónico para el nuevo objeto que está creando.</span><span class="sxs-lookup"><span data-stu-id="c3d18-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  