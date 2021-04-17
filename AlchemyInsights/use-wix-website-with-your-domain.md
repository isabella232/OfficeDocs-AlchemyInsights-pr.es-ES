---
title: Usar un sitio web de Wix con dominios comprados o administrados por Office 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825964"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Usar un sitio web de Wix con dominios comprados o administrados por Office 365

- [Actualizar registros DNS para conservar su sitio web con su proveedor de hospedaje actual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- El artículo de Wix "Conectar un dominio a Wix usando el método de señalización", recomienda usar la señalización (agregar registros DNS de acuerdo al vínculo anterior) en lugar de cambiar los servidores de nombres cuando use Office 365.
- Si, a pesar de todo, elige cambiar los servidores de nombres a Wix, entonces necesitará [crear los registros DNS en Wix para Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Si su dominio se compró a Microsoft, los servidores de nombres no se podrán cambiar. Si necesita cambiar los servidores de nombres, el dominio comprado de Microsoft debería [transferirse a otro proveedor de hospedaje después de 60 días](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)