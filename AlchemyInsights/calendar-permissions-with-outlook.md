---
title: Permisos de calendario
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854037"
---
# <a name="calendar-permissions"></a><span data-ttu-id="9230d-102">Permisos de calendario</span><span class="sxs-lookup"><span data-stu-id="9230d-102">Calendar Permissions</span></span>

<span data-ttu-id="9230d-103">Los usuarios pueden cambiar sus propios permisos de calendario con Outlook en la web u otros clientes, pero como administrador puede que también necesite investigar.</span><span class="sxs-lookup"><span data-stu-id="9230d-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="9230d-104">Con el cmdlet de PowerShell de Exchange se mostrará el permiso en el calendario de un usuario:</span><span class="sxs-lookup"><span data-stu-id="9230d-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="9230d-105">Para ver más información, consulte lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="9230d-105">To see more information see the following:</span></span>

- [<span data-ttu-id="9230d-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="9230d-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="9230d-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="9230d-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="9230d-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="9230d-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="9230d-109">Los permisos de calendario se usan en el uso compartido de calendarios, para ver más información sobre cómo compartir un calendario de Outlook, consulte estos artículos:</span><span class="sxs-lookup"><span data-stu-id="9230d-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="9230d-110">Compartir un calendario de Outlook con otras personas</span><span class="sxs-lookup"><span data-stu-id="9230d-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="9230d-111">Compartir el calendario en Outlook en la web para la empresa</span><span class="sxs-lookup"><span data-stu-id="9230d-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="9230d-112">Para solucionar problemas del permiso de calendario, puede usar la herramienta [Asistente para soporte y recuperación](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="9230d-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>