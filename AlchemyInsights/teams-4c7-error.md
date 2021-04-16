---
title: Error de Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786686"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="1f950-102">Error 4c7 en Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1f950-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="1f950-103">Este error se produce porque Microsoft Teams requiere autenticación de formularios.</span><span class="sxs-lookup"><span data-stu-id="1f950-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="1f950-104">Al implementar servicios de federación de Active Directory (AD FS), la autenticación de formularios no está habilitada para la intranet de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="1f950-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="1f950-105">Si se produce un error en la autenticación integrada de Windows, se te pedirá que inicies sesión con la autenticación de formularios.</span><span class="sxs-lookup"><span data-stu-id="1f950-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="1f950-106">Para resolver este problema, habilite la autenticación de formularios mediante el complemento AD FS Microsoft Management Console (MMC) en el equipo que tiene la copia local de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1f950-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="1f950-107">Para ello, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="1f950-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="1f950-108">En el panel de navegación, vaya a **Directivas de autenticación**.</span><span class="sxs-lookup"><span data-stu-id="1f950-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="1f950-109">En **Acciones** en el panel de detalles, seleccione **Editar autenticación principal global**.</span><span class="sxs-lookup"><span data-stu-id="1f950-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="1f950-110">En la **pestaña Intranet,** seleccione **Autenticación de formularios**.</span><span class="sxs-lookup"><span data-stu-id="1f950-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="1f950-111">Seleccione **Aceptar** (o **Aplicar**).</span><span class="sxs-lookup"><span data-stu-id="1f950-111">Select **OK** (or **Apply**).</span></span>