---
title: Enviar como carpeta pública habilitada para correo en EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394692"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="0d484-102">Carpeta pública habilitada para correo enviar como</span><span class="sxs-lookup"><span data-stu-id="0d484-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="0d484-103">En el siguiente ejemplo se asignan los permisos "enviar como" para la carpeta pública habilitada para correo NewPF1 al usuario Jason.</span><span class="sxs-lookup"><span data-stu-id="0d484-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="0d484-104">Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' sendas '</span><span class="sxs-lookup"><span data-stu-id="0d484-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="0d484-105">Para obtener información detallada acerca de la sintaxis y los parámetros, consulte [asignar los permisos "enviar como" o "enviar en nombre de" para las carpetas públicas habilitadas para correo](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="0d484-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>
