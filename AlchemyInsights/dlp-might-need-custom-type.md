---
title: DLP puede necesitar un tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030811"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP puede necesitar un tipo personalizado

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP puede requerir un tipo de información personalizado**

Con una directiva de prevención de pérdida de datos (DLP), puede identificar y proteger datos confidenciales en su organización. En algunos escenarios, es posible  que deba crear su propio tipo de información confidencial personalizada para proteger los datos de su organización.

Por ejemplo, es posible que su organización necesite identificar y proteger los id. de empleados u otros datos en algún formato específico de su organización. Si es así, vea los siguientes artículos para obtener más información.
  
 **Personalizar un tipo de información confidencial integrado**
  
Si un tipo de información confidencial integrado satisface sus necesidades con solo unos pocos retoques, puede personalizar un tipo de información [confidencial integrada.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por ejemplo, puede agregar o quitar palabras clave, o agregar o quitar evidencias de soporte, como una fecha o una dirección.
  
 **Crear un tipo personalizado de información confidencial**
  
Pero si necesitas identificar y proteger por completo un [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) tipo diferente de información confidencial, puedes crear un tipo de información confidencial personalizada en la interfaz de usuario del Centro de seguridad & cumplimiento.
  
**Crear un tipo personalizado de información confidencial en PowerShell del Centro de seguridad y cumplimientol**

Por último, si la interfaz de usuario no proporciona todas las opciones que necesita, puede crear un tipo de información confidencial personalizada en [PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)del Centro de seguridad & cumplimiento . Al empezar con un archivo XML, puede usar todas las opciones disponibles.
