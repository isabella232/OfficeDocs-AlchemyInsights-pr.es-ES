---
title: Regla DLP para el número de cuenta bancaria de EE. UU. no funciona
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005035"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemas de DLP con números de cuenta bancaria de EE. UU.

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemas de DLP con números de cuenta bancaria de EE. UU.**

¿Tiene problemas con la prevención de pérdida de datos  **(DLP)** que no funciona para el contenido que contiene un número de cuenta bancaria de ESTADOS UNIDOS al usar un tipo de información confidencial DLP en O365? Si es así, asegúrese de que el contenido contiene la información necesaria para lo que la directiva DLP está buscando cuando se evalúa.
  
Por ejemplo,  para una directiva de número de cuenta bancaria de ESTADOS UNIDOS configurada con un nivel de confianza del 85 %, se evalúan los siguientes elementos y se deben detectar para que la regla se desencadene:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** de 8 a 17 dígitos

- **[Patrón:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** de 8 a 17 dígitos consecutivos.

- **[Suma de comprobación:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, no hay suma de comprobación

- **[Definición:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Una directiva DLP está un 75 % segura de que ha detectado este tipo de información confidencial si, en una proximidad de 300 caracteres:

  - La expresión regular Regex_usa_bank_account_number encuentra contenido que coincida con el patrón

  - Se encuentra una palabra clave de Keyword_usa_Bank_Account.

    Por ejemplo, el siguiente ejemplo se desencadenaría para la directiva **número** de cuenta bancaria de Estados Unidos: Cuenta de 78344011

Para obtener más información sobre  lo que se necesita para que se detecte un número de cuenta bancaria de ESTADOS UNIDOS para su contenido, vea la siguiente sección de este artículo: Qué buscan los tipos de información confidencial para el número de cuenta bancaria de ESTADOS [UNIDOS](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Con otro tipo de información confidencial integrada, vea el siguiente artículo para obtener información sobre lo que se necesita para otros tipos: Qué buscan los tipos de [información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  