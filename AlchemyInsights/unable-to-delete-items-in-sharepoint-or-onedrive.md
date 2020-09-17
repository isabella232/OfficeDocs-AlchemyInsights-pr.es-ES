---
title: No se pueden eliminar elementos en SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806128"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="98e51-102">No se pueden eliminar los elementos</span><span class="sxs-lookup"><span data-stu-id="98e51-102">Unable to delete items</span></span>

<span data-ttu-id="98e51-103">Las directivas de retención pueden causar esto, tiene que deshabilitar o excluir la retención respectiva que está causando este problema.</span><span class="sxs-lookup"><span data-stu-id="98e51-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="98e51-104">Una vez quitada la retención o la Directiva de retención, el cambio puede tardar hasta 24 horas en surtir efecto.</span><span class="sxs-lookup"><span data-stu-id="98e51-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="98e51-105">Asegúrese de que no hay ninguna configuración de [Directiva de retención](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) en el elemento.</span><span class="sxs-lookup"><span data-stu-id="98e51-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="98e51-106">Es posible que el sitio haya superado el límite de almacenamiento, aumente la [cuota del sitio](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) y elimine el elemento.</span><span class="sxs-lookup"><span data-stu-id="98e51-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="98e51-107">Asegúrese de que otro usuario no ha [desprotegido](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) el elemento.</span><span class="sxs-lookup"><span data-stu-id="98e51-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="98e51-108">Por último, los administradores pueden usar [patrones y prácticas de SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), que contiene una biblioteca de comandos de PowerShell que le permiten realizar acciones de administración complejas, como forzar la eliminación de elementos stubborn.</span><span class="sxs-lookup"><span data-stu-id="98e51-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="98e51-109">Quitar archivo PNP</span><span class="sxs-lookup"><span data-stu-id="98e51-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="98e51-110">Quitar la carpeta PNP</span><span class="sxs-lookup"><span data-stu-id="98e51-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="98e51-111">Quitar elemento de lista PNP</span><span class="sxs-lookup"><span data-stu-id="98e51-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="98e51-112">Quitar lista PNP</span><span class="sxs-lookup"><span data-stu-id="98e51-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="98e51-113">Quitar campo PNP (columna)</span><span class="sxs-lookup"><span data-stu-id="98e51-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)