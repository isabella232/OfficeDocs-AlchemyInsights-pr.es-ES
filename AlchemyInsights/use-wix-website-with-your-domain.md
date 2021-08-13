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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980194"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Usar un sitio web de Wix con dominios comprados o administrados por Office 365

- [Actualizar registros DNS para conservar su sitio web con su proveedor de hospedaje actual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- El artículo de Wix "Conectar un dominio a Wix usando el método de señalización", recomienda usar la señalización (agregar registros DNS de acuerdo al vínculo anterior) en lugar de cambiar los servidores de nombres cuando use Office 365.
- Si, a pesar de todo, elige cambiar los servidores de nombres a Wix, entonces necesitará [crear los registros DNS en Wix para Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Si su dominio se compró a Microsoft, los servidores de nombres no se podrán cambiar. Si necesita cambiar los servidores de nombres, el dominio comprado de Microsoft debería [transferirse a otro proveedor de hospedaje después de 60 días](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)