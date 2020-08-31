---
title: Usar un sitio web de Wix con dominios comprados o administrados por Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300739"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Usar un sitio web de Wix con dominios comprados o administrados por Office 365

- [Actualizar registros DNS para conservar su sitio web con su proveedor de hospedaje actual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- El artículo de Wix "Conectar un dominio a Wix usando el método de señalización", recomienda usar la señalización (agregar registros DNS de acuerdo al vínculo anterior) en lugar de cambiar los servidores de nombres cuando usa Office 365
- Si a pesar de todo elige cambiar los servidores de nombres a Wix, entonces necesitará [crear los registros DNS en Wix para Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Si su dominio se compró desde Microsoft, los servidores de nombres no se pueden cambiar. Si necesita cambiar los servidores de nombres, el dominio comprado de Microsoft debería [transferirse a otro proveedor de hospedaje después de 60 días](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)