---
title: Configurar DKIM con dominios personalizados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737332"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurar DKIM con dominios personalizados

Debe publicar dos registros CNAME para cada dominio personalizado en DNS. Para ello, use el siguiente formato:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** es el texto a la izquierda de **.mail.protection.outlook.com** en el registro MX personalizado para el dominio personalizado (por ejemplo, contoso-com para el dominio **contoso.com**). **InitialDomain** es el dominio que usó cuando se inscribió en Office 365 (por ejemplo, **contoso.onmicrosoft.com**).

Para obtener más información acerca de los registros DNS, vea [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).