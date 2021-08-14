---
title: Regla DLP para número de pasaporte de ESTADOS UNIDOS/Reino Unido que no funciona
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004963"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas con DLP: números de pasaporte de Estados Unidos/Reino Unido

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemas de DLP con números de pasaporte de Estados Unidos/Reino Unido**

¿Tiene problemas con la prevención de pérdida de datos **(DLP)** que no funciona para el contenido que contiene un número de pasaporte de Estados **Unidos/Reino** Unido al usar un tipo de información confidencial DLP en O365? Si es así, asegúrese de que el contenido contiene la información necesaria para lo que la directiva DLP está buscando cuando se evalúa.
  
Por ejemplo, para una directiva de número de pasaporte de Estados **Unidos/Reino** Unido configurada con un nivel de confianza del 75 %, se evalúan los siguientes elementos y se deben detectar para que la regla se desencadene.
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nueve dígitos

- **[Patrón:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nueve dígitos consecutivos

- **[Suma de comprobación:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, no hay suma de comprobación

- **[Definición:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Una directiva DLP está un 75 % segura de que ha detectado este tipo de información confidencial si, en una proximidad de 300 caracteres:

  - La función Func_usa_uk_passport encuentra contenido que coincide con el patrón.

  - Se encuentra una palabra clave de Keyword_passport.

    Por ejemplo, el ejemplo siguiente se desencadenaría para la directiva de número de pasaporte de Estados **Unidos/Reino** Unido: número de pasaporte de EE.UU. 123456789

Para obtener más información sobre lo que se necesita para que se detecte un número de pasaporte de Estados Unidos/Reino Unido para su contenido, vea la siguiente sección de este artículo: Qué buscan los tipos de información confidencial para el número de pasaporte de Estados [Unidos/Reino Unido](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Con otro tipo de información confidencial integrada, vea el siguiente artículo para obtener información sobre lo que se necesita para otros tipos: Qué buscan los tipos de [información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  