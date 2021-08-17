---
title: Configurar DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108573"
---
# <a name="setup-dkim"></a>Configurar DKIM

Las instrucciones completas para configurar DKIM para dominios personalizados en Microsoft 365 están [aquí](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Para **cada** dominio personalizado, debe crear dos registros **DKIM** CNAME en el servicio de hospedaje DNS de su dominio (normalmente, el registrador de dominio). Por ejemplo, contoso.com y fourthcoffee.com requieren cuatro registros DKIM CNAME: dos para contoso.com y dos para fourthcoffee.com.

   Los registros CNAME DKIM para **cada** dominio personalizado usan los siguientes formatos:

   - **Nombre de host**: `selector1._domainkey.<CustomDomain>`

     **Apunta a dirección o valor:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nombre de host**: `selector2._domainkey.<CustomDomain>`

     **Apunta a dirección o valor:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> es el texto a la izquierda del registro MX personalizado para el dominio personalizado `.mail.protection.outlook.com` (por ejemplo, para el `contoso-com` dominio contoso.com). \<InitialDomain\>es el dominio que usó cuando se inscribió en Microsoft 365 (por ejemplo, contoso.onmicrosoft.com).

2. Después de crear los registros CNAME para los dominios personalizados, siga estas instrucciones:

   a. [inicie sesión en Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) con su cuenta laboral o educativa.

   b. Seleccione el icono del iniciador de aplicaciones en la esquina superior izquierda y elija **Administrador**.

   c. En el panel de navegación inferior izquierdo, expanda **Administración** y elija **Exchange**.

   d. Vaya a **Protección**  >  **DKIM**.

   e. Seleccione el dominio y, a continuación, **elija Habilitar** para firmar mensajes para este dominio con **firmas DKIM**. Repita este paso para cada dominio personalizado.
