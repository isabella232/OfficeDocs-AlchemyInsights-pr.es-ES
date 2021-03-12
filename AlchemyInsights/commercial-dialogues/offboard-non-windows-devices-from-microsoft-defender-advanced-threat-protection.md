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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737463"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="61edf-102">Dispositivos que no son de Windows de Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="61edf-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="61edf-103">A continuación se describe cómo:</span><span class="sxs-lookup"><span data-stu-id="61edf-103">Here's how:</span></span>

1. <span data-ttu-id="61edf-104">Siga la documentación de terceros para desconectar la solución de terceros de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="61edf-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="61edf-105">Desde el inquilino de Azure Active Directory, quite los permisos de la solución de terceros:</span><span class="sxs-lookup"><span data-stu-id="61edf-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="61edf-106">Inicie sesión en el [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="61edf-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="61edf-107">Seleccione **Todos los servicios** Azure Active  >  **Directory** Enterprise  >  **Applications**.</span><span class="sxs-lookup"><span data-stu-id="61edf-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="61edf-108">Selecciona la aplicación que quieras quitar.</span><span class="sxs-lookup"><span data-stu-id="61edf-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="61edf-109">Seleccione **Eliminar**.</span><span class="sxs-lookup"><span data-stu-id="61edf-109">Select **Delete**.</span></span>

<span data-ttu-id="61edf-110">Para obtener más información, [consulta Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="61edf-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
