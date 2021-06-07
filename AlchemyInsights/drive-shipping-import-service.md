---
title: 'Envío de unidades de disco en el servicio de importación de Microsoft 365 '
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721725"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="72899-102">Envío de unidades de disco en el servicio de importación de Microsoft 365 </span><span class="sxs-lookup"><span data-stu-id="72899-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="72899-103">Para usar el envío de unidades de disco, copie los archivos PST en una unidad de disco duro y, después, envíela a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72899-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="72899-104">Para empezar:</span><span class="sxs-lookup"><span data-stu-id="72899-104">To start the job:</span></span>

1. <span data-ttu-id="72899-105">En el Centro de cumplimiento de Microsoft 365, haga clic en **Gobierno de la información y** seleccione **Importar**.</span><span class="sxs-lookup"><span data-stu-id="72899-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="72899-106">Seleccione **Elegir tipo de trabajo de importación** y **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="72899-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="72899-107">Para ver los pasos de esta opción de importación, seleccione **Enviar unidades de disco duro a una de nuestras ubicaciones físicas**.</span><span class="sxs-lookup"><span data-stu-id="72899-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="72899-108">Aspectos que se deben tener en cuenta:</span><span class="sxs-lookup"><span data-stu-id="72899-108">Here are some things to remember:</span></span>

- <span data-ttu-id="72899-109">Debe tener asignada la función de importación y exportación de buzón en Exchange Online para importar archivos PST a los buzones de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72899-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="72899-110">El rendimiento puede verse afectado para archivos PST de más de 20 GB.</span><span class="sxs-lookup"><span data-stu-id="72899-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="72899-111">Solo se admiten unidades de estado sólido (SSD) de 2,5 pulgadas o discos duros internos SATA II/III de 2,5 o 3,5 pulgadas.</span><span class="sxs-lookup"><span data-stu-id="72899-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="72899-112">El disco duro con archivos PST se debe cifrar con BitLocker.</span><span class="sxs-lookup"><span data-stu-id="72899-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="72899-113">El costo de la importación de los archivos PST a los buzones de Microsoft 365 mediante el envío de unidades es de 2 $ por cada GB de datos.</span><span class="sxs-lookup"><span data-stu-id="72899-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="72899-114">Para obtener más información sobre el uso del método de envío de unidades para la importación de archivos PST, consulte[Usar el envío de unidades para importar los archivos PST de su organización](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="72899-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>