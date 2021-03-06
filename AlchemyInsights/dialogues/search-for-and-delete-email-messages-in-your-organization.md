---
title: Buscar y eliminar mensajes de correo electrónico en la organización
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500969"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="ac2bf-102">Buscar y eliminar mensajes de correo electrónico en la organización</span><span class="sxs-lookup"><span data-stu-id="ac2bf-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="ac2bf-103">Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="ac2bf-103">Follow these steps:</span></span>

1. <span data-ttu-id="ac2bf-104">Si no es un administrador global, para buscar mensajes, su  cuenta debe agregarse al grupo de roles administrador de exhibición de documentos electrónicos o al rol de administración **Búsqueda de cumplimiento**.</span><span class="sxs-lookup"><span data-stu-id="ac2bf-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="ac2bf-105">Para eliminar mensajes, deberá unirse al grupo de roles **Administración** de la organización o al rol **de administración Buscar y purgar**.</span><span class="sxs-lookup"><span data-stu-id="ac2bf-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="ac2bf-106">Los permisos para estos roles se asignan en el [Centro de seguridad & cumplimiento.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="ac2bf-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="ac2bf-107">[Cree una búsqueda de contenido](https://docs.microsoft.com/office365/securitycompliance/content-search) para buscar el mensaje que desea eliminar.</span><span class="sxs-lookup"><span data-stu-id="ac2bf-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="ac2bf-108">[Conéctese al Centro de seguridad y cumplimiento de PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ac2bf-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="ac2bf-109">Si usa MFA, consulte estas instrucciones: Conectarse a PowerShell del Centro de [seguridad & cumplimiento mediante la autenticación multifactor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="ac2bf-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="ac2bf-110">Eliminar el mensaje: ejecute el `New-ComplianceSearchAction` cmdlet para eliminar el mensaje.</span><span class="sxs-lookup"><span data-stu-id="ac2bf-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="ac2bf-111">Los mensajes eliminados se mueven a la carpeta Elementos recuperables de un usuario.</span><span class="sxs-lookup"><span data-stu-id="ac2bf-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="ac2bf-112">Para obtener un comando de ejemplo, vea [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="ac2bf-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
