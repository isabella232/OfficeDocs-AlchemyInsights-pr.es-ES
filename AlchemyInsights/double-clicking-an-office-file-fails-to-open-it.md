---
title: Al hacer doble clic en un archivo de Office no se puede abrir
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814822"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="3fac1-102">Al hacer doble clic en un archivo de Office no se puede abrir</span><span class="sxs-lookup"><span data-stu-id="3fac1-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="3fac1-103">Después de hacer doble clic en un archivo de Office, es posible que vea el programa abierto, pero el archivo en sí no se abre.</span><span class="sxs-lookup"><span data-stu-id="3fac1-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="3fac1-104">O puede obtener el error: "Hubo un problema al enviar el comando al programa".</span><span class="sxs-lookup"><span data-stu-id="3fac1-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="3fac1-105">Hay muchas causas para esto, pero las dos soluciones más comunes son:</span><span class="sxs-lookup"><span data-stu-id="3fac1-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="3fac1-106">Desde Excel, asegúrese de que la opción DDE está desactivada.</span><span class="sxs-lookup"><span data-stu-id="3fac1-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="3fac1-107">La opción se puede encontrar mediante la creación de un nuevo libro y, a continuación, eligiendo **Archivo > opciones > advanced**.</span><span class="sxs-lookup"><span data-stu-id="3fac1-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="3fac1-108">En la **sección General,** desactive omitir otras aplicaciones que **usan Dynamic Data Exchange (DDE).**</span><span class="sxs-lookup"><span data-stu-id="3fac1-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="3fac1-109">Ejecute una reparación en línea para restaurar la configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3fac1-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="3fac1-110">Haz clic en el botón Inicio de Windows y busca "Panel de control".</span><span class="sxs-lookup"><span data-stu-id="3fac1-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="3fac1-111">Abra el **Panel de control** y vaya a Programas > y **características**.</span><span class="sxs-lookup"><span data-stu-id="3fac1-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="3fac1-112">A continuación, **haga clic Microsoft Office [Versión]** y elija **Cambiar > Reparación en línea**.</span><span class="sxs-lookup"><span data-stu-id="3fac1-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="3fac1-113">Si ninguna de estas soluciones funciona, se puede encontrar una lista más completa de soluciones en el artículo de soporte técnico, al hacer doble clic en un archivo de [Office no](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)se puede abrir .</span><span class="sxs-lookup"><span data-stu-id="3fac1-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
