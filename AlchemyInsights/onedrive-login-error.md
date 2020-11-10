---
title: AADSTS50011 de error de inicio de sesión de OneDrive
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947533"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="e8b42-102">AADSTS50011 de error de inicio de sesión de OneDrive</span><span class="sxs-lookup"><span data-stu-id="e8b42-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="e8b42-103">Si recibe un error "AADSTS50011: la dirección URL de respuesta especificada en la solicitud no coincide con la respuesta" al iniciar sesión en la aplicación de OneDrive, compruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="e8b42-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="e8b42-104">La versión de OneDrive debe ser igual o mayor que la versión 20.052. XXXX. XXX.</span><span class="sxs-lookup"><span data-stu-id="e8b42-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="e8b42-105">Para comprobar la versión, haga clic en el icono azul de OneDrive del área de notificación, seleccione **ayuda & configuración > configuración > acerca de**.</span><span class="sxs-lookup"><span data-stu-id="e8b42-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="e8b42-106">La red podría bloquear el tráfico a **g.Live.com** y **oneclient.SFX.ms**.</span><span class="sxs-lookup"><span data-stu-id="e8b42-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="e8b42-107">Si se bloquea el tráfico, OneDrive no puede actualizarse a sí mismo.</span><span class="sxs-lookup"><span data-stu-id="e8b42-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="e8b42-108">Trabaje con el administrador de la red para asegurarse de que tiene acceso a esas direcciones URL.</span><span class="sxs-lookup"><span data-stu-id="e8b42-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="e8b42-109">[Estos extremos](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) deben ser accesibles para los clientes que usen planes de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8b42-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="e8b42-110">Si necesita obtener manualmente una versión actual de OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="e8b42-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
