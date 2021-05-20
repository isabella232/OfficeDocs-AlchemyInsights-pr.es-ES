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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539841"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="00a9b-102">Falta correo electrónico en cuarentena"</span><span class="sxs-lookup"><span data-stu-id="00a9b-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="00a9b-103">Los administradores [pueden ver, liberar o eliminar estos mensajes.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="00a9b-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="00a9b-104">Para abrir el Centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="00a9b-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="00a9b-105">Para abrir la página Cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="00a9b-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="00a9b-106">Puede buscar según los siguientes valores:</span><span class="sxs-lookup"><span data-stu-id="00a9b-106">You can search by the following values:</span></span>  

- <span data-ttu-id="00a9b-107">**Id. de mensaje**: El identificador único global del mensaje.</span><span class="sxs-lookup"><span data-stu-id="00a9b-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="00a9b-108">Si selecciona un mensaje en la lista, el  valor **id.** de mensaje aparece en el panel desplegable Detalles que aparece.</span><span class="sxs-lookup"><span data-stu-id="00a9b-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="00a9b-109">Los administradores pueden usar [seguimiento de mensajes](/microsoft-365/security/office-365-security/message-trace-scc) para buscar mensajes y los valores de Id. de mensaje correspondientes.</span><span class="sxs-lookup"><span data-stu-id="00a9b-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="00a9b-110">**Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.</span><span class="sxs-lookup"><span data-stu-id="00a9b-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="00a9b-111">**Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.</span><span class="sxs-lookup"><span data-stu-id="00a9b-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="00a9b-112">**Asunto**: Use el asunto completo del mensaje.</span><span class="sxs-lookup"><span data-stu-id="00a9b-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="00a9b-113">La búsqueda no distingue entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="00a9b-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="00a9b-114">Cuando haya introducido los criterios de búsqueda, haga clic en ![Botón actualizar](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualizar** para filtrar los resultados.</span><span class="sxs-lookup"><span data-stu-id="00a9b-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="00a9b-115">Los cmdlets que usa para ver y administrar mensajes y archivos en cuarentena son:</span><span class="sxs-lookup"><span data-stu-id="00a9b-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="00a9b-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00a9b-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="00a9b-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00a9b-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="00a9b-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00a9b-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="00a9b-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)tenga en cuenta que este cmdlet solo es para mensajes, no archivos de malware de Microsoft Defender para Office 365 para SharePoint Online, OneDrive para la Empresa o Teams.</span><span class="sxs-lookup"><span data-stu-id="00a9b-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="00a9b-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00a9b-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)