---
title: Es posible que DLP necesite un tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507531"
---
# <a name="dlp-might-need-a-custom-type"></a>Es posible que DLP necesite un tipo personalizado

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Es posible que DLP requiera un tipo de información personalizada**

Con una directiva de prevención de pérdida de datos (DLP), puede identificar y proteger los datos confidenciales de su organización. En algunos escenarios, es posible que necesite crear su propio tipo **personalizado** de información confidencial para proteger los datos de su organización.

Por ejemplo, es posible que su organización necesite identificar y proteger los identificadores de los empleados u otros datos en algún formato específico de su organización. Si es así, consulte los artículos siguientes para obtener más información.
  
 **Personalizar un tipo de información confidencial integrado**
  
Si un tipo de información confidencial incorporado satisface sus necesidades con solo unos cuantos ajustes, puede [personalizar un tipo de información confidencial integrada](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Por ejemplo, puede Agregar o quitar palabras clave, o bien agregar o quitar evidencias auxiliares, como una fecha o una dirección.
  
 **Crear un tipo personalizado de información confidencial**
  
Pero si necesita identificar y proteger por completo un tipo diferente de información confidencial, puede [crear un tipo personalizado de información confidencial](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) en la interfaz de usuario del centro de seguridad & cumplimiento.
  
**Crear un tipo personalizado de información confidencial en PowerShell del Centro de seguridad y cumplimientol**

Por último, si la interfaz de usuario no proporciona todas las opciones que necesita, puede [crear un tipo personalizado de información confidencial en el PowerShell del centro de cumplimiento de & de seguridad](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Al comenzar con un archivo XML, puede usar todas las opciones disponibles.
