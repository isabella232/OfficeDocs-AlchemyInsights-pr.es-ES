---
title: Creación y uso compartido de calendarios de carpetas públicas en Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: bec11baa2de7154481ec175df2466eb601b0e243
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903623"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="48474-102">Creación y uso compartido de calendarios de carpetas públicas en Exchange Online</span><span class="sxs-lookup"><span data-stu-id="48474-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="48474-103">Solo se puede crear un calendario en una carpeta pública desde el cliente de escritorio de Outlook.</span><span class="sxs-lookup"><span data-stu-id="48474-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="48474-104">Siga estos pasos para configurar calendarios de carpetas públicas:</span><span class="sxs-lookup"><span data-stu-id="48474-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="48474-105">Compruebe que las carpetas públicas están implementadas en Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="48474-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="48474-106">Para obtener más información, consulte [Crear un buzón de carpetas públicas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="48474-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="48474-107">Compruebe que tiene asignados los permisos de acceso necesarios para crear la carpeta pública.</span><span class="sxs-lookup"><span data-stu-id="48474-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="48474-108">Para obtener más información, consulte [Permisos de carpetas públicas de Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="48474-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="48474-109">Inicie sesión en el cliente de escritorio de Outlook y compruebe que puede acceder a la implementación de la carpeta pública.</span><span class="sxs-lookup"><span data-stu-id="48474-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="48474-110">Si tiene problemas para acceder a carpetas públicas con el cliente de escritorio de Outlook, consulte [Los usuarios de Exchange Online no se pueden conectar a carpetas públicas mediante Outlook o OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="48474-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="48474-111">Cree un nuevo tipo de calendario para la carpeta pública.</span><span class="sxs-lookup"><span data-stu-id="48474-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="48474-112">La carpeta pública se comparte con el resto de usuarios de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="48474-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="48474-113">El propietario de la carpeta pública puede modificar los permisos desde el cliente de escritorio de Outlook.</span><span class="sxs-lookup"><span data-stu-id="48474-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="48474-114">Para obtener más información, consulte [Permisos de carpetas públicas de Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="48474-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="48474-115">**Nota:** Los calendarios de carpetas públicas están diseñados para usarse dentro de las organizaciones, por lo que no se pueden publicar en Internet.</span><span class="sxs-lookup"><span data-stu-id="48474-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="48474-116">Use un buzón compartido si lo que quiere es publicar un calendario en Internet.</span><span class="sxs-lookup"><span data-stu-id="48474-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>