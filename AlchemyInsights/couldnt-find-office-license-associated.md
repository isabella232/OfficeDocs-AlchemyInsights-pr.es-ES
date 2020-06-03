---
title: Solución de aplicaciones de Office no se pudo encontrar el mensaje asociado de licencias de Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505884"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="e63c4-102">Corrección del mensaje "no se pudieron encontrar las licencias de Office asociadas" en las aplicaciones de Office</span><span class="sxs-lookup"><span data-stu-id="e63c4-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="e63c4-103">Si recibe este mensaje, pruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="e63c4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e63c4-104">Compruebe el firewall, el software antivirus y la configuración de proxy para confirmar que no están bloqueando el acceso a Internet a las aplicaciones de Office.</span><span class="sxs-lookup"><span data-stu-id="e63c4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e63c4-105">Consulte [direcciones URL e intervalos de direcciones IP de 365 de Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e63c4-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="e63c4-106">Quite y [reasigne la licencia de Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) para el usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="e63c4-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="e63c4-107">Abra una aplicación de Office y [cierre la sesión](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) de las cuentas de usuario existentes.</span><span class="sxs-lookup"><span data-stu-id="e63c4-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="e63c4-108">Vaya a configuración de Windows **> cuentas**de  >  **correo &** cuentas y quite todas las cuentas de trabajo excepto la cuenta afectada.</span><span class="sxs-lookup"><span data-stu-id="e63c4-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="e63c4-109">Vaya a configuración de Windows > **cuentas**  >  **tienen acceso a trabajo o escuela**y desconectan todas las cuentas de trabajo, excepto la cuenta afectada.</span><span class="sxs-lookup"><span data-stu-id="e63c4-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="e63c4-110">Restablezca el estado de activación de Office.</span><span class="sxs-lookup"><span data-stu-id="e63c4-110">Reset the Office activation state.</span></span> <span data-ttu-id="e63c4-111">[Obtenga más información](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e63c4-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="e63c4-112">[Inicie sesión](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con la cuenta de usuario afectada.</span><span class="sxs-lookup"><span data-stu-id="e63c4-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="e63c4-113">Para obtener soluciones adicionales para la solución de problemas, consulte [errores de activación y de producto sin licencia en Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="e63c4-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>