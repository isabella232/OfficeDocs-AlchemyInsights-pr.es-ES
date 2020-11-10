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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947534"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="5dd68-102">Comentarios en elementos de lista</span><span class="sxs-lookup"><span data-stu-id="5dd68-102">Comments on List items</span></span>

<span data-ttu-id="5dd68-103">Los usuarios pronto podrán agregar y eliminar comentarios en los elementos de lista.</span><span class="sxs-lookup"><span data-stu-id="5dd68-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="5dd68-104">Los usuarios pueden ver todos los comentarios de un elemento de lista y filtrar entre las vistas que muestran comentarios o actividades relacionadas con un elemento.</span><span class="sxs-lookup"><span data-stu-id="5dd68-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="5dd68-105">**Intervalos** :</span><span class="sxs-lookup"><span data-stu-id="5dd68-105">**Timing** :</span></span>

<span data-ttu-id="5dd68-106">**Versión dirigida** : implementación gradual en mediados de octubre y prevista para completar a mediados de noviembre</span><span class="sxs-lookup"><span data-stu-id="5dd68-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="5dd68-107">**Versión estándar** : implementación gradual en Mid-noviembre y espera que finalice antes de diciembre</span><span class="sxs-lookup"><span data-stu-id="5dd68-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="5dd68-108">**Implementación** : versión dirigida para toda la organización</span><span class="sxs-lookup"><span data-stu-id="5dd68-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="5dd68-109">Los usuarios deben tener en cuenta lo siguiente para poder agregar y eliminar comentarios:</span><span class="sxs-lookup"><span data-stu-id="5dd68-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="5dd68-110">Los comentarios siguen la configuración de permisos inherente a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5dd68-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="5dd68-111">Las listas clásicas que aún no se han creado para que se muestren en las interfaces de usuario modernas, como las listas de tareas, no tendrán esta característica de comentarios.</span><span class="sxs-lookup"><span data-stu-id="5dd68-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="5dd68-112">La publicación de comentarios sobre listas en Microsoft Teams no está disponible en esta versión.</span><span class="sxs-lookup"><span data-stu-id="5dd68-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="5dd68-113">Los comentarios no se indizan mediante la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="5dd68-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="5dd68-114">Los administradores pueden deshabilitar esta característica en el nivel de la organización cambiando el parámetro **CommentsOnListItemsDisabled** en el cmdlet de PowerShell **set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="5dd68-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="5dd68-115">Actualmente no se pueden deshabilitar los comentarios en el nivel de sitio o lista.</span><span class="sxs-lookup"><span data-stu-id="5dd68-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="5dd68-116">Esperamos que esos controles estén en una actualización posterior, probablemente en el primer trimestre del 2021.</span><span class="sxs-lookup"><span data-stu-id="5dd68-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
