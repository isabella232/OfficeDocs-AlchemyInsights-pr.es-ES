---
title: Regla DLP para el número de tarjeta de crédito que no funciona
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005107"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemas de DLP con números de tarjeta de crédito

**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemas de DLP con números de tarjeta de crédito**

¿Tiene problemas con la prevención de pérdida de datos  **(DLP)** que no funciona para el contenido que contiene un número de tarjeta de crédito al usar un tipo de información confidencial DLP en O365? Si es así, asegúrese de que el contenido contiene la información necesaria para desencadenar la directiva DLP cuando se evalúe. Por ejemplo, para una directiva **de tarjeta** de crédito configurada con un nivel de confianza del 85 %, se evalúan lo siguiente y se deben detectar para que la regla se desencadene:
  
- **[Formato:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 dígitos que pueden tener formato o sin formato (ddddddddddddd) y deben pasar la prueba de Luhn.

- **[Patrón:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Patrón muy complejo y robusto que detecta tarjetas de todas las principales marcas del mundo, incluidas Visa, MasterCard, Discover Card, JCB, American Express, tarjetas de regalo y tarjetas de comensal.

- **[Suma de comprobación:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Sí, la suma de comprobación de Luhn

- **[Definición:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Una directiva DLP está 85 % segura de que ha detectado este tipo de información confidencial si, en una proximidad de 300 caracteres:

  - La función Func_credit_card encuentra contenido que coincide con el patrón.

  - Una de las siguientes opciones es verdadera:

  - Se encuentra una palabra clave de Keyword_cc_verification.

  - Se encuentra una palabra Keyword_cc_name de la página

  - La función Func_expiration_date encuentra una fecha en el formato de fecha correcto.

  - La suma de comprobación pasa

    Por ejemplo, el ejemplo siguiente se desencadenaría para una directiva de número de tarjeta de crédito DLP:

  - Visa: 4485 3647 3952 7352
  
  - Expira: 2/2009

Para obtener más información sobre  lo que se necesita para que se detecte un número de tarjeta de crédito para su contenido, vea la siguiente sección de este artículo: ¿Qué buscan los tipos de información confidencial para la tarjeta de [crédito#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Con otro tipo de información confidencial integrada, vea el siguiente artículo para obtener información sobre lo que se necesita para otros tipos: Qué buscan los tipos de [información confidencial](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  