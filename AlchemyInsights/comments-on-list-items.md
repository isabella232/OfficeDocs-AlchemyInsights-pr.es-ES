---
title: Comentarios en elementos de lista
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724171"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="463e4-102">Comentarios en elementos de lista</span><span class="sxs-lookup"><span data-stu-id="463e4-102">Comments on List items</span></span>

<span data-ttu-id="463e4-103">Los usuarios pueden ver todos los comentarios de un elemento de lista y filtrar entre las vistas que muestran comentarios o actividades relacionadas con un elemento.</span><span class="sxs-lookup"><span data-stu-id="463e4-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="463e4-104">Los usuarios deben tener en cuenta lo siguiente para poder agregar y eliminar comentarios:</span><span class="sxs-lookup"><span data-stu-id="463e4-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="463e4-105">Los comentarios siguen la configuración de permisos inherente a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="463e4-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="463e4-106">Las listas clásicas que aún no se han creado para que se muestren en las interfaces de usuario modernas, como las listas de tareas, no tendrán esta característica de comentarios.</span><span class="sxs-lookup"><span data-stu-id="463e4-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="463e4-107">La publicación de comentarios sobre listas en Microsoft Teams no está disponible en esta versión.</span><span class="sxs-lookup"><span data-stu-id="463e4-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="463e4-108">Los comentarios no se indizan mediante la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="463e4-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="463e4-109">Los administradores pueden deshabilitar esta característica en el nivel de la organización cambiando el parámetro **CommentsOnListItemsDisabled** en el cmdlet de PowerShell **set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="463e4-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="463e4-110">Actualmente no se pueden deshabilitar los comentarios en el nivel de sitio o lista.</span><span class="sxs-lookup"><span data-stu-id="463e4-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="463e4-111">Esperamos que esos controles estén en una actualización posterior, probablemente en el primer trimestre del 2021.</span><span class="sxs-lookup"><span data-stu-id="463e4-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
