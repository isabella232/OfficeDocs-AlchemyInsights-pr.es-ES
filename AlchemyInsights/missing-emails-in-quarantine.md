---
title: Falta correo electrónico en cuarentena
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
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831751"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="eab4c-102">Falta correo electrónico en cuarentena"</span><span class="sxs-lookup"><span data-stu-id="eab4c-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="eab4c-103">Los administradores [pueden ver, liberar o eliminar estos mensajes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="eab4c-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="eab4c-104">Para abrir el Centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="eab4c-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="eab4c-105">Para abrir la página Cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="eab4c-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="eab4c-106">Puede buscar según los siguientes valores:</span><span class="sxs-lookup"><span data-stu-id="eab4c-106">You can search by the following values:</span></span>  

- <span data-ttu-id="eab4c-107">**Id. de mensaje**: El identificador único global del mensaje.</span><span class="sxs-lookup"><span data-stu-id="eab4c-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="eab4c-108">Si selecciona un mensaje en la lista, el  valor **id.** de mensaje aparece en el panel desplegable Detalles que aparece.</span><span class="sxs-lookup"><span data-stu-id="eab4c-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="eab4c-109">Los administradores pueden usar [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para buscar mensajes y los valores de Id. de mensaje correspondientes.</span><span class="sxs-lookup"><span data-stu-id="eab4c-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="eab4c-110">**Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.</span><span class="sxs-lookup"><span data-stu-id="eab4c-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="eab4c-111">**Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.</span><span class="sxs-lookup"><span data-stu-id="eab4c-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="eab4c-112">**Asunto**: Use el asunto completo del mensaje.</span><span class="sxs-lookup"><span data-stu-id="eab4c-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="eab4c-113">La búsqueda no distingue entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="eab4c-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="eab4c-114">Después de especificar los criterios de búsqueda, haga clic ![ en el botón Actualizar ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **para** filtrar los resultados.  </span><span class="sxs-lookup"><span data-stu-id="eab4c-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="eab4c-115">Los cmdlets que usa para ver y administrar mensajes y archivos en cuarentena son:</span><span class="sxs-lookup"><span data-stu-id="eab4c-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="eab4c-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="eab4c-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="eab4c-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="eab4c-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="eab4c-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="eab4c-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="eab4c-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)tenga en cuenta que este cmdlet solo es para mensajes, no archivos de malware de ATP para SharePoint Online, OneDrive para la Empresa o Teams.</span><span class="sxs-lookup"><span data-stu-id="eab4c-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="eab4c-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="eab4c-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)