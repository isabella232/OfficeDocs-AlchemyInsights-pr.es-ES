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
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232815"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="a1d52-102">Bloquear firmas de correo electrónico realizadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="a1d52-102">Block user-made email signatures</span></span>

<span data-ttu-id="a1d52-103">La siguiente solución solo se aplica a las firmas de correo electrónico creadas en Outlook en la Web.</span><span class="sxs-lookup"><span data-stu-id="a1d52-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="a1d52-104">Solo puede bloquear firmas en la aplicación de Outlook si tiene una aplicación local Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a1d52-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="a1d52-105">En el centro de administración, elija **Centros de administración de**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="a1d52-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="a1d52-106">Haga **clic en permisos directivas** de Outlook Web  >  **App**.</span><span class="sxs-lookup"><span data-stu-id="a1d52-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="a1d52-107">Seleccione la directiva y, a continuación, haga clic en el icono de lápiz para editarla.</span><span class="sxs-lookup"><span data-stu-id="a1d52-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="a1d52-108">Características **de clic** Más  >  **opciones.**</span><span class="sxs-lookup"><span data-stu-id="a1d52-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="a1d52-109">En **Experiencia del usuario,** desactive la casilla **Firma** de correo electrónico y, a continuación, haga clic **en Guardar.**</span><span class="sxs-lookup"><span data-stu-id="a1d52-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="a1d52-110">**Importante:** Si se agregó una firma antes de desactivar esta casilla, el usuario podrá usarla.</span><span class="sxs-lookup"><span data-stu-id="a1d52-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="a1d52-111">Pídales que lo quiten.</span><span class="sxs-lookup"><span data-stu-id="a1d52-111">Ask them to remove it.</span></span>
