---
title: Corregir aplicaciones de Microsoft 365 No se pudo encontrar el mensaje asociado a licencias de office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816505"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="fd2cd-102">Corregir el mensaje de aplicaciones de Microsoft 365 "No se pudieron encontrar licencias de office asociadas"</span><span class="sxs-lookup"><span data-stu-id="fd2cd-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="fd2cd-103">Si recibe este mensaje, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="fd2cd-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fd2cd-104">Comprueba la configuración del firewall, el software antivirus y el proxy para confirmar que no bloquean el acceso a Internet a las aplicaciones de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fd2cd-105">Consulte Direcciones URL e intervalos de direcciones IP de [Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fd2cd-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="fd2cd-106">Quitar y [reasignar la licencia de Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para el usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="fd2cd-107">Abra una aplicación de Office y [salga de](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) cualquier cuenta de usuario existente.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="fd2cd-108">Ve a Configuración de Windows > **Cuentas** de correo & cuentas y quita todas las cuentas de trabajo  >  excepto la cuenta afectada.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="fd2cd-109">Ve a Configuración de Windows > **Acceso a** cuentas laborales o educativas y desconecta todas las cuentas de trabajo excepto la  >  cuenta afectada.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="fd2cd-110">Restablezca el estado de activación de Office.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-110">Reset the Office activation state.</span></span> <span data-ttu-id="fd2cd-111">[Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="fd2cd-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="fd2cd-112">[Inicie sesión](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.</span><span class="sxs-lookup"><span data-stu-id="fd2cd-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="fd2cd-113">Para obtener soluciones de solución de problemas adicionales, vea Errores de activación y productos sin [licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="fd2cd-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>