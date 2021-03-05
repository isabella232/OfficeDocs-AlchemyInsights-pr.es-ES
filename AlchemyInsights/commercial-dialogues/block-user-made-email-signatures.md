---
title: Bloquear firmas de correo electrónico realizadas por el usuario
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464873"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="f9a8b-102">Bloquear firmas de correo electrónico realizadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="f9a8b-102">Block user-made email signatures</span></span>

<span data-ttu-id="f9a8b-103">La siguiente solución solo se aplica a las firmas de correo electrónico creadas en Outlook en la web.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="f9a8b-104">Solo puede bloquear firmas en la aplicación de Outlook si tiene un Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="f9a8b-105">En el Centro de administración, elija **Centros de administración**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="f9a8b-106">Haga **clic en permisos Directivas** de Outlook Web  >  **App**.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="f9a8b-107">Seleccione la directiva y, a continuación, haga clic en el icono de lápiz para editarla.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="f9a8b-108">Características **de clic** Más  >  **opciones**.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="f9a8b-109">En **Experiencia del usuario,** desactive la casilla **Firma de** correo electrónico y, a continuación, haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="f9a8b-110">**Importante:** Si se agregó una firma antes de desactivar esta casilla, el usuario podrá usarla.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="f9a8b-111">Pídales que lo quiten.</span><span class="sxs-lookup"><span data-stu-id="f9a8b-111">Ask them to remove it.</span></span>
