---
title: DLP no funciona como se esperaba
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079719"
---
# <a name="dlp-not-working-as-expected"></a>DLP no funciona como se esperaba

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Configuración de DLP**

¿Tiene problemas con prevención de pérdida de datos **(DLP)** en Office 365 no funciona como se esperaba? Si es así, asegúrese de que la directiva **DLP** está configurada correctamente y de que los datos contienen lo que la directiva **DLP** está buscando cuando se está evaluando.
  
Las directivas DLP le permiten identificar y proteger información confidencial en su organización. Para configurar directivas DLP, use la información [aquí](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Qué buscan las directivas DLP**
  
Al usar los **tipos de** información confidencial integrados en los centros de seguridad y cumplimiento, las directivas DLP buscan patrones y elementos específicos al detectar estos tipos confidenciales.
  
- **Tipos de información confidencial integrados**

    Para obtener información sobre los tipos confidenciales integrados y lo que busca una directiva DLP al detectar el tipo confidencial, vea: Qué buscan los tipos de información [confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipos de información confidencial personalizados**

    Si está intentando crear tipos de información confidencial personalizados, use el siguiente artículo para obtener información sobre cómo crear un tipo confidencial personalizado: Crear un tipo de información [confidencial personalizada](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Probar una directiva DLP**

Para probar los datos con un tipo de información  confidencial integrada o personalizada, use la opción Tipo de prueba en **Clasificaciones**  >  **Tipos de información confidencial**. Para obtener más información, vea [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Informes**
  
- Obtenga información sobre datos confidenciales con [informes DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Vea detalles específicos del evento con un [informe de incidentes](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
