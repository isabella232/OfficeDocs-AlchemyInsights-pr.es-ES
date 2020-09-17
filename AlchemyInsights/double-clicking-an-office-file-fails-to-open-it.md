---
title: No se puede abrir el doble clic en un archivo de Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812096"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="95dfc-102">No se puede abrir el doble clic en un archivo de Office</span><span class="sxs-lookup"><span data-stu-id="95dfc-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="95dfc-103">Después de hacer doble clic en un archivo de Office, puede ver que el programa está abierto pero el archivo no se abre.</span><span class="sxs-lookup"><span data-stu-id="95dfc-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="95dfc-104">O puede que reciba el error: "hubo un problema al enviar el comando al programa".</span><span class="sxs-lookup"><span data-stu-id="95dfc-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="95dfc-105">Hay muchas causas para esto, pero las dos soluciones más comunes son:</span><span class="sxs-lookup"><span data-stu-id="95dfc-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="95dfc-106">En Excel, asegúrese de que la opción DDE esté desactivada.</span><span class="sxs-lookup"><span data-stu-id="95dfc-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="95dfc-107">Puede encontrar la opción si crea un libro nuevo y, a continuación, elige **Opciones de > de archivos > avanzadas**.</span><span class="sxs-lookup"><span data-stu-id="95dfc-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="95dfc-108">En la sección **General** , desactive la casilla **Omitir otras aplicaciones que usen el intercambio dinámico de datos (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="95dfc-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="95dfc-109">Ejecute una reparación en línea para restaurar la configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="95dfc-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="95dfc-110">Haga clic en el botón Inicio de Windows y busque "panel de control".</span><span class="sxs-lookup"><span data-stu-id="95dfc-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="95dfc-111">Abra el **Panel de control**y vaya a **programas > programas y características**.</span><span class="sxs-lookup"><span data-stu-id="95dfc-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="95dfc-112">A continuación, haga clic con el botón secundario en **Microsoft Office [versión]** y elija **cambiar > reparación en línea**.</span><span class="sxs-lookup"><span data-stu-id="95dfc-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="95dfc-113">Si ninguna de estas soluciones funciona, puede encontrar una lista más completa de soluciones en el artículo de soporte técnico, al [hacer doble clic en un archivo de Office se produce un error al abrirlo](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="95dfc-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
