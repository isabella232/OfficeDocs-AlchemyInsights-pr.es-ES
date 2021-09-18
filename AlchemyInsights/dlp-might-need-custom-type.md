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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446708"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP puede necesitar un tipo personalizado

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP puede requerir un tipo de información personalizado**

Con una directiva de prevención de pérdida de datos (DLP), puede identificar y proteger datos confidenciales en su organización. En algunos escenarios, es posible que deba crear su propio tipo de información confidencial personalizada para proteger los datos de su organización. Para obtener más información, vea [Learn about sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) and Sensitive information type entity [definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Para obtener más información sobre cómo crear directivas y tipos de información confidencial personalizados, vea: 

**Personalizar un tipo de información confidencial integrado**

Si un tipo de información confidencial integrado satisface sus necesidades con solo unos pocos retoques, vea Personalizar un tipo de información [confidencial integrada.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por ejemplo, puede agregar o quitar palabras clave, o agregar o quitar evidencias de soporte, como una fecha o una dirección.

**Crear un tipo personalizado de información confidencial**

Pero si necesita identificar y proteger por completo un tipo diferente de información confidencial, puede crear un tipo de información confidencial personalizado en el Centro de cumplimiento de Microsoft 365. Para obtener más información, vea [Introducción a los tipos de información confidencial personalizados.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Crear un tipo personalizado de información confidencial en PowerShell del Centro de seguridad y cumplimientol**

Por último, si la interfaz de usuario no proporciona todas las opciones que necesita, puede crear un tipo de información confidencial personalizada en PowerShell del Centro de seguridad & cumplimiento. Al empezar con un archivo XML, puede usar todas las opciones disponibles. Para obtener más información, vea [Create a custom sensitive information type using PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Para probar primero la directiva en modo de prueba, vea [Implement policy in test mode](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) y [Create, test, and tune a DLP policy](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 