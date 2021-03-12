---
title: Solucionar problemas de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707971"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="1d815-102">Solucionar problemas de acceso denegado de mensajes en El Centro de administración de Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="1d815-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="1d815-103">Si recibe un mensaje de acceso denegado al intentar navegar a un Centro de administración de Sharepoint/OneDrive, asegúrese de asignar una licencia [al usuario](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="1d815-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="1d815-104">Si el usuario tiene una licencia, también debe asegurarse de que se les asigna un rol de [administrador](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) que pueda tener acceso a los centros de administración.</span><span class="sxs-lookup"><span data-stu-id="1d815-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="1d815-105">Este problema también puede producirse cuando un usuario se elimina y se vuelve a crear con el mismo nombre principal de usuario (UPN).</span><span class="sxs-lookup"><span data-stu-id="1d815-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="1d815-106">La nueva cuenta se crea mediante un valor puid (identificador único de Passport) diferente.</span><span class="sxs-lookup"><span data-stu-id="1d815-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="1d815-107">Cuando el usuario intenta obtener acceso a una colección de sitios o a su OneDrive, el usuario tiene un PUID incorrecto.</span><span class="sxs-lookup"><span data-stu-id="1d815-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="1d815-108">Un segundo escenario implica la sincronización de directorios con una unidad organizativa (OU) de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1d815-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="1d815-109">Si los usuarios ya han iniciado sesión en SharePoint y, a continuación, se mueven a otra unidad organizativa y se vuelve a sincronizar con SharePoint, pueden experimentar este problema.</span><span class="sxs-lookup"><span data-stu-id="1d815-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="1d815-110">Para resolver este problema, debe restaurar el UPN original con los pasos descritos en el artículo Restaurar [un usuario en Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="1d815-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="1d815-111">Nota: Si un Centro de administración de OneDrive o SharePoint no está disponible para varios usuarios que tenían acceso anteriormente, puede haber un problema de servicio temporal.</span><span class="sxs-lookup"><span data-stu-id="1d815-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="1d815-112">[Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1d815-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


