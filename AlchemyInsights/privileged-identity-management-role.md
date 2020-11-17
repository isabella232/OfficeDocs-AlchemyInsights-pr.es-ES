---
title: Rol de administración de identidades con privilegios
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086377"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="961e9-102">Rol de administración de identidades privilegiada (PIM)</span><span class="sxs-lookup"><span data-stu-id="961e9-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="961e9-103">**No se conceden permisos tras activar un rol**</span><span class="sxs-lookup"><span data-stu-id="961e9-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="961e9-104">Al activar un rol en Azure AD privileged Identity Management (PIM), es posible que la activación no se propague inmediatamente a todos los portales que requieran el rol privilegiado.</span><span class="sxs-lookup"><span data-stu-id="961e9-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="961e9-105">A veces, incluso si se propaga el cambio, el almacenamiento en caché de Web en un portal puede hacer que el cambio no surta efecto inmediatamente.</span><span class="sxs-lookup"><span data-stu-id="961e9-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="961e9-106">Si la activación se retrasa, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="961e9-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="961e9-107">Cierre la sesión de Azure portal y, a continuación, vuelva a iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="961e9-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="961e9-108">Al activar un rol de Azure AD o un rol de recurso de Azure, verá las fases de la activación.</span><span class="sxs-lookup"><span data-stu-id="961e9-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="961e9-109">Una vez completadas todas las etapas, verá el vínculo "cerrar sesión".</span><span class="sxs-lookup"><span data-stu-id="961e9-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="961e9-110">Puede usar este vínculo para cerrar la sesión. Esto resolverá la mayoría de los casos para el retraso de la activación.</span><span class="sxs-lookup"><span data-stu-id="961e9-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="961e9-111">En PIM, compruebe que se encuentra como miembro de la función.</span><span class="sxs-lookup"><span data-stu-id="961e9-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="961e9-112">Si está activando el rol de administrador de Exchange, asegúrese de cerrar la sesión y volver a iniciarla.</span><span class="sxs-lookup"><span data-stu-id="961e9-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="961e9-113">Si el problema persiste, abra una incidencia de soporte técnico y provoque esto como un problema.</span><span class="sxs-lookup"><span data-stu-id="961e9-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="961e9-114">Si usa el rol de administrador de Exchange para tener acceso al centro de seguridad y cumplimiento, consulte el paso siguiente.</span><span class="sxs-lookup"><span data-stu-id="961e9-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="961e9-115">Si está activando un rol para obtener acceso al centro de seguridad y cumplimiento o si está activando el rol de administrador de SharePoint, experimentará algunos retrasos en la activación desde hace unos minutos, hasta unas horas.</span><span class="sxs-lookup"><span data-stu-id="961e9-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="961e9-116">Se trata de un problema conocido y estamos trabajando activamente con estos equipos para resolver este problema tan pronto como sea posible.</span><span class="sxs-lookup"><span data-stu-id="961e9-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="961e9-117">Para más información, vea:</span><span class="sxs-lookup"><span data-stu-id="961e9-117">For more information, see:</span></span>

- [<span data-ttu-id="961e9-118">Activar mis roles de Azure AD en PIM</span><span class="sxs-lookup"><span data-stu-id="961e9-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="961e9-119">Activar mis roles de recursos de Azure en PIM</span><span class="sxs-lookup"><span data-stu-id="961e9-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="961e9-120">**Los permisos no se quitan después de desactivar una función o la activación de la función expira**</span><span class="sxs-lookup"><span data-stu-id="961e9-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="961e9-121">Cuando se desactiva un rol en la administración de identidades privilegiada de Azure AD o cuando expira un período de activación de rol, es posible que se produzca un retraso en el que continúe teniendo acceso.</span><span class="sxs-lookup"><span data-stu-id="961e9-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="961e9-122">Si la desactivación se retrasa, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="961e9-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="961e9-123">Si está desactivando el rol de administrador de Exchange o el período de activación de roles expira y observa un retraso significativo antes de que se quiten los permisos, abra un vale de soporte técnico y dígale a su ingeniero de soporte técnico que le ayude a archivar un vale con el equipo de administración de acceso privilegiado (PAM) en Office sobre este problema.</span><span class="sxs-lookup"><span data-stu-id="961e9-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="961e9-124">Si ha expirado el período de activación, pero todavía tiene la sesión del explorador abierta, cierre el explorador.</span><span class="sxs-lookup"><span data-stu-id="961e9-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="961e9-125">Puede seguir usando el rol hasta que cierre esa sesión.</span><span class="sxs-lookup"><span data-stu-id="961e9-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="961e9-126">Se trata de un problema conocido y estamos examinando una solución potencial para revocar activamente cada sesión una vez que la activación haya expirado.</span><span class="sxs-lookup"><span data-stu-id="961e9-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="961e9-127">Si el retraso es distinto de estos dos escenarios, abra una incidencia de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="961e9-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
