---
title: Preguntas sobre cómo usar la herramienta Office implementación (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959700"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Preguntas sobre cómo usar la herramienta Office implementación (ODT)

Descargue la Herramienta de implementación de Office desde el [Centro de descarga de Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Después de descargar el archivo autoextraíble, ejecútelo para extraer el archivo ejecutable de la Herramienta de implementación de Office (setup.exe) y un archivo de configuración de ejemplo (configuration.xml).
  
 **Para excluir o quitar productos Aplicaciones Microsoft 365 para empresas de los equipos cliente:**
  
Al instalar Aplicaciones Microsoft 365 para empresas, puede excluir productos específicos. Para hacerlo, siga los pasos para instalar Office con la ODT, pero incluya el elemento ExcludeApp en el archivo de configuración. Por ejemplo, este archivo de configuración instala todos los Aplicaciones Microsoft 365 para empresas excepto Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Información general sobre la Herramienta de implementación de Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

