---
title: Preguntas sobre cómo usar la Herramienta de implementación de Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790349"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="8cebf-102">Preguntas sobre cómo usar la Herramienta de implementación de Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="8cebf-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="8cebf-103">Descargue la Herramienta de implementación de Office desde el [Centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="8cebf-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="8cebf-104">Después de descargar el archivo autoextraíble, ejecútelo para extraer el archivo ejecutable de la Herramienta de implementación de Office (setup.exe) y un archivo de configuración de ejemplo (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="8cebf-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="8cebf-105">**Para excluir o quitar aplicaciones de Microsoft 365 para productos empresariales de los equipos cliente:**</span><span class="sxs-lookup"><span data-stu-id="8cebf-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="8cebf-106">Al instalar Aplicaciones de Microsoft 365 para empresas, puede excluir productos específicos.</span><span class="sxs-lookup"><span data-stu-id="8cebf-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="8cebf-107">Para hacerlo, siga los pasos para instalar Office con la ODT, pero incluya el elemento ExcludeApp en el archivo de configuración.</span><span class="sxs-lookup"><span data-stu-id="8cebf-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="8cebf-108">Por ejemplo, este archivo de configuración instala todas las aplicaciones de Microsoft 365 para productos empresariales excepto Publisher:</span><span class="sxs-lookup"><span data-stu-id="8cebf-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="8cebf-109">Información general sobre la Herramienta de implementación de Office</span><span class="sxs-lookup"><span data-stu-id="8cebf-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

