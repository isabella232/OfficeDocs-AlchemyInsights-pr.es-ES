---
title: Mensajes de correo electrónico que faltan en cuarentena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673731"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="a6de2-102">Mensajes que faltan en cuarentena</span><span class="sxs-lookup"><span data-stu-id="a6de2-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="a6de2-103">Los administradores pueden [ver, liberar o eliminar estos mensajes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a6de2-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="a6de2-104">Para abrir el centro de seguridad & cumplimiento, vaya a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="a6de2-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="a6de2-105">Para abrir la página de cuarentena directamente, vaya a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="a6de2-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="a6de2-106">Puede buscar según los siguientes valores:</span><span class="sxs-lookup"><span data-stu-id="a6de2-106">You can search by the following values:</span></span>  

- <span data-ttu-id="a6de2-107">**Id. de mensaje**: El identificador único global del mensaje.</span><span class="sxs-lookup"><span data-stu-id="a6de2-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="a6de2-108">Si selecciona un mensaje de la lista, el valor del  **identificador de mensaje**  aparece en el panel flotante de  **detalles**  que aparece.</span><span class="sxs-lookup"><span data-stu-id="a6de2-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="a6de2-109">Los administradores pueden usar [seguimiento de mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) para buscar mensajes y los valores de Id. de mensaje correspondientes.</span><span class="sxs-lookup"><span data-stu-id="a6de2-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="a6de2-110">**Dirección de correo electrónico del remitente**: Una única dirección de correo electrónico de remitente.</span><span class="sxs-lookup"><span data-stu-id="a6de2-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="a6de2-111">**Dirección de correo electrónico del destinatario**: Una única dirección de correo electrónico de destinatario.</span><span class="sxs-lookup"><span data-stu-id="a6de2-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="a6de2-112">**Asunto**: Use el asunto completo del mensaje.</span><span class="sxs-lookup"><span data-stu-id="a6de2-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="a6de2-113">La búsqueda no distingue entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a6de2-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="a6de2-114">Una vez que haya introducido los criterios de búsqueda, haga clic en ![ Actualizar botón ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualizar** para filtrar los resultados.  </span><span class="sxs-lookup"><span data-stu-id="a6de2-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="a6de2-115">Los cmdlets que se usan para ver y administrar mensajes y archivos en cuarentena son los siguientes:</span><span class="sxs-lookup"><span data-stu-id="a6de2-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="a6de2-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a6de2-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="a6de2-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a6de2-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="a6de2-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a6de2-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="a6de2-119">[Vista previa de QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): tenga en cuenta que este cmdlet solo es para los mensajes, no para los archivos de malware de ATP para SharePoint Online, OneDrive para la empresa o Teams.</span><span class="sxs-lookup"><span data-stu-id="a6de2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="a6de2-120">Versión-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="a6de2-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)