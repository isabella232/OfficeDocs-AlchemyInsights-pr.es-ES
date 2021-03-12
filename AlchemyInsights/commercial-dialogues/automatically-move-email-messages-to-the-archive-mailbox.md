---
title: Mover automáticamente mensajes de correo electrónico al buzón de archivo
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737587"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="f2c40-102">Mover automáticamente mensajes de correo electrónico al buzón de archivo</span><span class="sxs-lookup"><span data-stu-id="f2c40-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="f2c40-103">Este es el modo de configurar una directiva para mover automáticamente el correo electrónico antiguo de un usuario al buzón de archivo:</span><span class="sxs-lookup"><span data-stu-id="f2c40-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="f2c40-104">Vaya a [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data governance Archive para comprobar que se ha habilitado un buzón de archivo para el  >    >   usuario.</span><span class="sxs-lookup"><span data-stu-id="f2c40-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="f2c40-105">Si no lo ha hecho, haga clic **en Habilitar** **y,** a continuación, en Sí en el cuadro de advertencia.</span><span class="sxs-lookup"><span data-stu-id="f2c40-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="f2c40-106">Vaya al [**Centro de administración de Exchange > administración de cumplimiento > etiquetas de retención**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="f2c40-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="f2c40-107">Elija el icono + y, a **continuación, elija aplicar automáticamente a todo el buzón**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="f2c40-108">Asigne un nombre a la etiqueta de retención y elija **Mover a Archivo**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="f2c40-109">Para el período de retención, escriba el tiempo que desee, como 90 días.</span><span class="sxs-lookup"><span data-stu-id="f2c40-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="f2c40-110">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-110">Click **Save**.</span></span>
5. <span data-ttu-id="f2c40-111">Ahora cree una directiva de retención: elija **directivas de retención,** elija el icono para agregar una nueva directiva.</span><span class="sxs-lookup"><span data-stu-id="f2c40-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="f2c40-112">Asigne un nombre a la directiva de retención y, a continuación, haga clic y desplácese para buscar y agregar la etiqueta de retención que acaba de crear.</span><span class="sxs-lookup"><span data-stu-id="f2c40-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="f2c40-113">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-113">Click **Save**.</span></span>
7. <span data-ttu-id="f2c40-114">Por último, aplique la directiva de retención al buzón del usuario: aún en el Centro de administración de Exchange, vaya a **buzones**  >  **de destinatarios**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="f2c40-115">Elija todos los usuarios a los que desea aplicar la directiva y, a continuación, **elija Editar** (icono de lápiz).</span><span class="sxs-lookup"><span data-stu-id="f2c40-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="f2c40-116">En el cuadro de diálogo, haga clic **en Características del buzón**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="f2c40-117">En **Directiva de retención,** aplique la directiva que acaba de crear > **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f2c40-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="f2c40-118">Para obtener instrucciones para aplicar la directiva a todos los usuarios, vea [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="f2c40-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
