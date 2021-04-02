---
title: Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo unido a un dominio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426893"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="0e12e-102">Establecer Microsoft Edge como el explorador web predeterminado en un dispositivo unido a un dominio</span><span class="sxs-lookup"><span data-stu-id="0e12e-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="0e12e-103">Establecer Microsoft Edge como explorador web predeterminado:</span><span class="sxs-lookup"><span data-stu-id="0e12e-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="0e12e-104">[Cree un archivo de configuración de asociaciones predeterminado](https://go.microsoft.com/fwlink/?linkid=2132437) y guárdelo localmente o en un recurso compartido de red.</span><span class="sxs-lookup"><span data-stu-id="0e12e-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="0e12e-105">Abra el editor de Directivas de grupo y a continuación, vaya a **Configuración del equipo** > **Plantillas administrativas** > **Componentes de Windows** > **Explorador de archivos**.</span><span class="sxs-lookup"><span data-stu-id="0e12e-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="0e12e-106">Seleccione **Establecer un archivo de configuración de asociaciones predeterminado**.</span><span class="sxs-lookup"><span data-stu-id="0e12e-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="0e12e-107">Seleccione **Configuración de directivas** y después seleccione **Habilitado**.</span><span class="sxs-lookup"><span data-stu-id="0e12e-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="0e12e-108">En **Opciones**, escriba la ubicación del archivo de configuración de asociaciones predeterminado y, a continuación, seleccione **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="0e12e-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
