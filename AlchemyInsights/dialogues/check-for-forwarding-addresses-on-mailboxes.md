---
title: Buscar direcciones de reenvío en buzones
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417229"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="7daad-102">Buscar direcciones de reenvío en buzones</span><span class="sxs-lookup"><span data-stu-id="7daad-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="7daad-103">A veces, los hackers reenvían los mensajes de correo electrónico de los usuarios a sí mismos, por lo que primero comprobaremos si hay direcciones de reenvío y reglas en el buzón.</span><span class="sxs-lookup"><span data-stu-id="7daad-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="7daad-104">A continuación, comprobaremos los registros de auditoría.</span><span class="sxs-lookup"><span data-stu-id="7daad-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="7daad-105">Este es el modo de comprobar las direcciones de reenvío:</span><span class="sxs-lookup"><span data-stu-id="7daad-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="7daad-106">Seleccione **Usuarios**  >  **Usuarios activos**.</span><span class="sxs-lookup"><span data-stu-id="7daad-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="7daad-107">Seleccione el usuario cuya cuenta se ha visto comprometida.</span><span class="sxs-lookup"><span data-stu-id="7daad-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="7daad-108">En el control desplegable que aparece, expanda **Configuración de correo** y, a continuación, haga clic en **Editar** para reenvío de **correo electrónico.**</span><span class="sxs-lookup"><span data-stu-id="7daad-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="7daad-109">Quite las direcciones de reenvío que no reconozca.</span><span class="sxs-lookup"><span data-stu-id="7daad-109">Remove any forwarding addresses you don't recognize.</span></span>