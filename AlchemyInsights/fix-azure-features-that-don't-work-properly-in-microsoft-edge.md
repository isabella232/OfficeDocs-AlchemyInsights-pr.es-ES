---
title: Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576599"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="2773d-102">Qué hacer si las características de Azure no funcionan correctamente en Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2773d-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="2773d-103">Microsoft Edge tiene [problemas conocidos](https://go.microsoft.com/fwlink/?linkid=2140608) relacionados con las zonas de seguridad y pueden afectar al modo en que los usuarios de Azure inician sesión en el centro de administración de Windows.</span><span class="sxs-lookup"><span data-stu-id="2773d-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="2773d-104">Si tienes problemas para usar las características de Azure con Microsoft Edge, prueba los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="2773d-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="2773d-105">En el menú **Inicio** , busque **Opciones de Internet** y selecciónela.</span><span class="sxs-lookup"><span data-stu-id="2773d-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="2773d-106">En el cuadro de diálogo **propiedades de Internet** , vaya a la ficha **seguridad** .</span><span class="sxs-lookup"><span data-stu-id="2773d-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="2773d-107">Seleccione la zona **sitios de confianza** y, a continuación, seleccione el botón **sitios** .</span><span class="sxs-lookup"><span data-stu-id="2773d-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="2773d-108">En el cuadro de diálogo **sitios de confianza** , agregue la dirección URL de la puerta de enlace, así como [https://login.microsoftonline.com](https://login.microsoftonline.com) y y [https://login.live.com](https://login.live.com) , a continuación, seleccione **cerrar**.</span><span class="sxs-lookup"><span data-stu-id="2773d-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="2773d-109">En el cuadro de diálogo **propiedades de Internet** , vaya a la pestaña **privacidad** .</span><span class="sxs-lookup"><span data-stu-id="2773d-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="2773d-110">En la sección **bloqueador de ventanas emergentes** , seleccione **configuración**.</span><span class="sxs-lookup"><span data-stu-id="2773d-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="2773d-111">En el cuadro de diálogo que se abre, agregue la dirección URL de la puerta de enlace, así como [https://login.microsoftonline.com](https://login.microsoftonline.com) y y [https://login.live.com](https://login.live.com) , a continuación, seleccione **cerrar**.</span><span class="sxs-lookup"><span data-stu-id="2773d-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
