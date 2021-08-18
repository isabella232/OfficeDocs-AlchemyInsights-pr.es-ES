---
title: Limitaciones de las etiquetas de confidencialidad de los archivos de Office en SharePoint y OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e2fc8fcf27eb916f64e4235cd116d9a7096e6078391e72363421ac3de721f5ee
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899781"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitaciones de las etiquetas de confidencialidad de los archivos de Office en SharePoint y OneDrive

Al habilitar etiquetas de confidencialidad para archivos de Office en SharePoint y OneDrive, tenga en cuenta los requisitos y limitaciones, que incluyen:

- SharePoint y OneDrive no pueden procesar algunos archivos etiquetados y cifrados desde aplicaciones de escritorio de Office cuando los archivos contienen datos de PowerQuery, datos almacenados por complementos personalizados o elementos XML personalizados.
- SharePoint y OneDrive no aplican etiquetas de confidencialidad de forma automática a los archivos existentes que ya ha cifrado con etiquetas de Azure Information Protection (AIP). Para aplicar etiquetas de confidencialidad a archivos cifrados: 
    - Asegúrese de que las etiquetas de AIP se han migrado y publicado en el Centro de cumplimiento de Microsoft 365.
    - Descargue los archivos etiquetados y cárguelos en su ubicación original de SharePoint o OneDrive.
- En el caso de los documentos cifrados, no se admite la impresión.

Para más información sobre las limitaciones, vea [Habilitar etiquetas de confidencialidad para los archivos de Office en SharePoint y OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
