---
title: Cómo agregar o quitar un delegado en Outlook para Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571910"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="f8cd7-102">Cómo agregar o quitar un delegado en Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="f8cd7-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="f8cd7-103">Para agregar un delegado en Outlook para Windows:</span><span class="sxs-lookup"><span data-stu-id="f8cd7-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="f8cd7-104">Haga clic en la pestaña **archivo** seguida de **configuración** de la cuenta y, a continuación, elija **delegar acceso**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="f8cd7-105">Haga clic en **Agregar**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-105">Click on **Add**.</span></span> <span data-ttu-id="f8cd7-106">Si no aparece **Agregar** , es posible que no exista una conexión activa entre Outlook y Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="f8cd7-107">La barra de estado de Outlook muestra el estado de la conexión.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="f8cd7-108">Escriba el nombre de la persona que desea designar como su delegado, o bien busque y elija el nombre en la lista de resultados de la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f8cd7-109">El delegado debe ser una persona de la lista global de direcciones (GAL) de Exchange de la organización.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="f8cd7-110">Haga clic en **Agregar** seguido de **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="f8cd7-111">En el cuadro de diálogo **permisos de delegado** , acepte la configuración de permisos predeterminada o seleccione niveles de acceso personalizados para las carpetas de Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="f8cd7-112">Si un delegado necesita permiso para trabajar solo con convocatorias de reunión y respuestas, la configuración de permisos predeterminada, como **Delegate recibe copias de los mensajes de reunión que se me envíen** es suficiente.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="f8cd7-113">Puede dejar la configuración de permisos de la **bandeja de entrada** en **ninguno**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="f8cd7-114">Las convocatorias de reunión y las respuestas Irán directamente a la bandeja de entrada del delegado.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f8cd7-115">De forma predeterminada, el delegado tiene concedido el permiso **Editor (puede leer, crear y modificar elementos)** a la carpeta **calendario** .</span><span class="sxs-lookup"><span data-stu-id="f8cd7-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="f8cd7-116">Cuando el delegado responde a una reunión en su nombre, se agrega automáticamente a la carpeta del **calendario** .</span><span class="sxs-lookup"><span data-stu-id="f8cd7-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="f8cd7-117">Para enviar un mensaje para notificar al delegado los permisos modificados, active la casilla de verificación **enviar automáticamente un mensaje al delegado que resume estos permisos** .</span><span class="sxs-lookup"><span data-stu-id="f8cd7-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="f8cd7-118">Si lo desea, active la casilla el **delegado puede ver mis elementos privados** .</span><span class="sxs-lookup"><span data-stu-id="f8cd7-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="f8cd7-119">Esta configuración afecta a todas las carpetas de Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="f8cd7-120">Esto incluye todas las carpetas correo, contactos, calendario, tareas, notas y diario.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="f8cd7-121">No hay ninguna forma de conceder acceso a los elementos privados en las carpetas especificadas.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="f8cd7-122">Elija **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="f8cd7-123">Los mensajes enviados con los permisos enviar en nombre de incluyen el delegado y los nombres junto a **desde**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="f8cd7-124">Cuando se envía un mensaje con los permisos enviar como, sólo aparece su nombre.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="f8cd7-125">Una vez que agregue a alguien como delegado, puede Agregar el buzón de Exchange a su perfil de Outlook.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="f8cd7-126">Para obtener instrucciones, consulte [administrar los elementos de correo y calendario de otra persona](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="f8cd7-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="f8cd7-127">Para quitar un delegado en Outlook para Windows:</span><span class="sxs-lookup"><span data-stu-id="f8cd7-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="f8cd7-128">Haga clic en la pestaña **archivo** .</span><span class="sxs-lookup"><span data-stu-id="f8cd7-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="f8cd7-129">Haga clic en configuración de la **cuenta** seguida de **Acceso delegado**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="f8cd7-130">Elija el nombre del delegado para el que desea cambiar los permisos y, a continuación, haga clic en **quitar** seguida de **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="f8cd7-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
