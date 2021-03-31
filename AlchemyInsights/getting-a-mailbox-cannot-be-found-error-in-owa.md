---
title: 126 ¿No se puede encontrar un error de obtención de un buzón en OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426679"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="9ba4e-102">¿No se encontró un error de buzón en Outlook en la web?</span><span class="sxs-lookup"><span data-stu-id="9ba4e-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="9ba4e-103">Si usa Outlook en la web y obtiene un buzón no se pudo encontrar por **error,** la cuenta que usó para conectarse a Outlook en la web no tiene una licencia de Exchange Online y, por lo tanto, no hay ningún buzón asociado a la cuenta.</span><span class="sxs-lookup"><span data-stu-id="9ba4e-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="9ba4e-104">El administrador puede asignar una licencia a su cuenta siguiendo estos pasos:</span><span class="sxs-lookup"><span data-stu-id="9ba4e-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="9ba4e-105">Abra el [Centro de administración de Microsoft 365](https://portal.office.com/adminportal/home#/homepage) y vaya a **Usuarios** activos en la sección Usuarios y seleccione el usuario que ve el error. </span><span class="sxs-lookup"><span data-stu-id="9ba4e-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="9ba4e-106">En la página de usuario  que se abre, vaya  a la sección Licencias y aplicaciones, seleccione el valor de ubicación adecuado y asigne una licencia que contenga Exchange Online (expanda la licencia para ver sus detalles).</span><span class="sxs-lookup"><span data-stu-id="9ba4e-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="9ba4e-107">Cuando haya terminado, haga clic en **Guardar cambios**.</span><span class="sxs-lookup"><span data-stu-id="9ba4e-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="9ba4e-108">En algunos casos, si la licencia ya está asignada a una cuenta de usuario, quitar y reasignar la licencia ayuda a resolver el problema y a aprovisionar correctamente en el sistema:</span><span class="sxs-lookup"><span data-stu-id="9ba4e-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="9ba4e-109">Compruebe si sus suscripciones de M365 Exchange Online (y otras, si tiene alguna) están actualizadas y no han expirado recientemente.</span><span class="sxs-lookup"><span data-stu-id="9ba4e-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="9ba4e-110">Una vez que haya asegurado que la suscripción no ha expirado y que se ha asignado una licencia válida a la cuenta de usuario, la licencia puede tardar hasta 24 horas en aprovisionarse, por lo que es posible que tenga que esperar a que se resuelva el problema.</span><span class="sxs-lookup"><span data-stu-id="9ba4e-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="9ba4e-111">Para obtener más información, consulta [Asignar y administrar licencias.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="9ba4e-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>