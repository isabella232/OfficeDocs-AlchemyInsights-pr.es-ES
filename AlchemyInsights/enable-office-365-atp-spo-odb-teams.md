---
title: Habilitar Office 365 ATP para SharePoint, OneDrive y Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543945"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="de5e2-102">Habilitar Microsoft Defender para Office 365 para SharePoint Online, OneDrive y Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="de5e2-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="de5e2-103">Vaya a https://protection.office.com e inicie sesión.</span><span class="sxs-lookup"><span data-stu-id="de5e2-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="de5e2-104">Elija **Directiva de administración**  >  **de** amenazas Caja fuerte datos  >  **adjuntos**.</span><span class="sxs-lookup"><span data-stu-id="de5e2-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="de5e2-105">Seleccione Activar Defender para Office 365 para **SharePoint, OneDrive y Microsoft Teams** y, a continuación, haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="de5e2-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="de5e2-106">(Recomendado) Como administrador global o administrador de SharePoint Online, ejecute el cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con el parámetro **DisallowInfectedFileDownload** establecido en *true*.</span><span class="sxs-lookup"><span data-stu-id="de5e2-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="de5e2-107">(Recomendado) [Configurar alertas para](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) archivos detectados.</span><span class="sxs-lookup"><span data-stu-id="de5e2-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="de5e2-108">Microsoft Defender para Office 365 examinará todos los archivos de SharePoint Online, OneDrive o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="de5e2-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="de5e2-109">Los archivos se examinan de forma asincrónica, a través de un proceso que usa eventos de actividad de invitado y uso compartido, junto con heurística inteligente y señales de amenazas para identificar archivos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="de5e2-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="de5e2-110">Consulta [Microsoft Defender para Office 365 para SharePoint, OneDrive y Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="de5e2-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>