---
title: Regla DLP para SSN que no funciona
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004999"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemas de DLP con números de seguridad social

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemas de DLP con SSN**

¿Tiene problemas con la prevención de pérdida de datos **(DLP)** que no funciona para el contenido que contiene un número de seguridad **social (SSN)** al usar un tipo de información confidencial en Microsoft 365? Si es así, asegúrese de que el contenido contiene la información necesaria para lo que busca la directiva DLP. 
  
Por ejemplo, para una directiva de SSN configurada con un nivel de confianza del 85 %, se evalúan los siguientes elementos y se deben detectar para que la regla se desencadene:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 dígitos, que puede estar en un patrón con formato o sin formato

- **[Patrón:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cuatro funciones buscan SSN en cuatro patrones diferentes:

  - Func_ssn busca SSN con formato seguro anteriores a 2011 y formateados con guiones o espacios (ddd-dd-dddd O ddd dd dddd)

  - Func_unformatted_ssn busca SSN con formato seguro anteriores a 2011 y formateados de manera no específica como nueve dígitos consecutivos (ddddddddd)

  - Func_randomized_formatted_ssn busca SSN posteriores a 2011 y formateados con guiones o espacios (ddd-dd-dddd O ddd dd dddd)

  - Func_randomized_unformatted_ssn busca SSN posteriores a 2011 y formateados de manera no específica como nueve dígitos consecutivos (ddddddddd)

- **[Suma de comprobación:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, no hay suma de comprobación

- **[Definición:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Una directiva DLP está 85 % segura de que ha detectado este tipo de información confidencial si, en una proximidad de 300 caracteres:

  - La [función Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) encuentra contenido que coincida con el patrón.

  - Se encuentra una palabra clave de [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn). Algunos ejemplos de palabras clave son:  *Seguridad social, Seguridad social#, Soc Sec ,SSN*  . Por ejemplo, el ejemplo siguiente se desencadenaría para la directiva SSN dlp: **SSN: 489-36-8350**
  
Para obtener más información sobre lo que se necesita para que los SSN se detecten para el contenido, vea la siguiente sección de este artículo: Qué buscan los tipos de información confidencial para [los SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Con otro tipo de información confidencial integrada, vea el siguiente artículo para obtener información sobre lo que se necesita para otros tipos: Qué buscan los tipos de [información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  