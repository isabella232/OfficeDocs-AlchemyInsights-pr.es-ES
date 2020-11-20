---
title: Recuperar o reemplazar un mensaje de correo electrónico
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353523"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="9e977-102">Recuperar o reemplazar un mensaje de correo electrónico en Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9e977-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="9e977-103">Solo puede **recuperar los mensajes que se envían a las personas de su organización**.</span><span class="sxs-lookup"><span data-stu-id="9e977-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9e977-104">Por ejemplo, si el mensaje se envió a una dirección de gmail, no puede recuperarlo.</span><span class="sxs-lookup"><span data-stu-id="9e977-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="9e977-105">Solo puede **recuperar los mensajes enviados desde Outlook para el equipo**.</span><span class="sxs-lookup"><span data-stu-id="9e977-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="9e977-106">Si un usuario envía un mensaje con Outlook para Mac o Outlook en la web, no puede recuperarlo.</span><span class="sxs-lookup"><span data-stu-id="9e977-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="9e977-107">Como administrador de inquilinos, puede **recuperar mensajes en nombre de los usuarios mediante PowerShell** (para obtener más información, consulte: [Buscar y eliminar mensajes de correo electrónico](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="9e977-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="9e977-108">No puede recuperar mensajes del centro de administración.</span><span class="sxs-lookup"><span data-stu-id="9e977-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="9e977-109">Desplácese hacia abajo hasta "buscar y eliminar mensajes de correo electrónico de la organización" para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="9e977-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="9e977-110">**Recuperar o reemplazar un mensaje de correo electrónico enviado**</span><span class="sxs-lookup"><span data-stu-id="9e977-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="9e977-111">En el panel de carpetas de la izquierda de la ventana de Outlook, elija la carpeta elementos enviados.</span><span class="sxs-lookup"><span data-stu-id="9e977-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="9e977-112">Abra el mensaje que desea recuperar.</span><span class="sxs-lookup"><span data-stu-id="9e977-112">Open the message that you want to recall.</span></span> <span data-ttu-id="9e977-113">Debe hacer doble clic para abrir el mensaje.</span><span class="sxs-lookup"><span data-stu-id="9e977-113">You must double-click to open the message.</span></span> <span data-ttu-id="9e977-114">La selección del mensaje para que aparezca en el panel de lectura no le permitirá recuperar el mensaje.</span><span class="sxs-lookup"><span data-stu-id="9e977-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="9e977-115">En la pestaña mensaje, seleccione **acciones**  >  **recuperar este mensaje**.</span><span class="sxs-lookup"><span data-stu-id="9e977-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="9e977-116">Elija **eliminar copias no leídas de este mensaje** o **eliminar copias no leídas y reemplazarlas por un nuevo mensaje** y, a continuación, seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="9e977-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="9e977-117">Si va a enviar un mensaje de reemplazo, Redacte el mensaje y, a continuación, seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="9e977-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="9e977-118">El éxito o el fracaso de una recuperación de mensajes depende de la configuración de los destinatarios en Outlook.</span><span class="sxs-lookup"><span data-stu-id="9e977-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="9e977-119">Para obtener más información, incluido cómo comprobar la recuperación, vea [recuperar o reemplazar un mensaje de correo electrónico enviado](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9e977-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9e977-120">**_Para buscar y eliminar mensajes de correo electrónico en su organización_**, es más fácil si es un administrador global. Si no es un administrador global, su cuenta debe agregarse al grupo de roles eDiscovery Manager o al rol de administración de búsqueda de cumplimiento.</span><span class="sxs-lookup"><span data-stu-id="9e977-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="9e977-121">Para eliminar mensajes, debe unirse al grupo de funciones de administración de la organización o al rol de administración de búsqueda y depuración.</span><span class="sxs-lookup"><span data-stu-id="9e977-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9e977-122">Los permisos para estos roles se asignan en el [centro de seguridad & cumplimiento](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9e977-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="9e977-123">[Cree una búsqueda de contenido](https://docs.microsoft.com/microsoft-365/compliance/content-search) para buscar el mensaje que se va a eliminar.</span><span class="sxs-lookup"><span data-stu-id="9e977-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="9e977-124">[Conéctese al Centro de seguridad y cumplimiento de PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9e977-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="9e977-125">Si usa MFA (multi-factor Authentication), consulte [conectarse a Microsoft 365 Security & el centro de cumplimiento de PowerShell con multi-factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9e977-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
