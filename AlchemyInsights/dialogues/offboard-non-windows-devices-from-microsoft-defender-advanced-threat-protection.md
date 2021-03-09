---
title: Dispositivos que no son de Windows de Microsoft Defender Advanced Threat Protection (ATP)
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
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530218"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c93b5-102">Dispositivos que no son de Windows de Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="c93b5-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c93b5-103">A continuación se describe cómo:</span><span class="sxs-lookup"><span data-stu-id="c93b5-103">Here's how:</span></span>

1. <span data-ttu-id="c93b5-104">Siga la documentación de terceros para desconectar la solución de terceros de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="c93b5-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c93b5-105">Desde el inquilino de Azure Active Directory, quite los permisos de la solución de terceros:</span><span class="sxs-lookup"><span data-stu-id="c93b5-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c93b5-106">Inicie sesión en el [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="c93b5-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c93b5-107">Seleccione **Todos los servicios** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="c93b5-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c93b5-108">Selecciona la aplicación que quieras quitar.</span><span class="sxs-lookup"><span data-stu-id="c93b5-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c93b5-109">Seleccione **Eliminar**.</span><span class="sxs-lookup"><span data-stu-id="c93b5-109">Select **Delete**.</span></span>

<span data-ttu-id="c93b5-110">Para obtener más información, [consulta Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="c93b5-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
