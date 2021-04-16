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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Preguntas sobre cómo usar la Herramienta de implementación de Office (ODT)

Descargue la Herramienta de implementación de Office desde el [Centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Después de descargar el archivo autoextraíble, ejecútelo para extraer el archivo ejecutable de la Herramienta de implementación de Office (setup.exe) y un archivo de configuración de ejemplo (configuration.xml).
  
 **Para excluir o quitar aplicaciones de Microsoft 365 para productos empresariales de los equipos cliente:**
  
Al instalar Aplicaciones de Microsoft 365 para empresas, puede excluir productos específicos. Para hacerlo, siga los pasos para instalar Office con la ODT, pero incluya el elemento ExcludeApp en el archivo de configuración. Por ejemplo, este archivo de configuración instala todas las aplicaciones de Microsoft 365 para productos empresariales excepto Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Información general sobre la Herramienta de implementación de Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

