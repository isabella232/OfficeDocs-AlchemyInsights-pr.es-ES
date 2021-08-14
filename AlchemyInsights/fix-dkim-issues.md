---
title: Corregir problemas de instalación de DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945948"
---
# <a name="fix-dkim-setup-issues"></a>Corregir problemas de instalación de DKIM

Si tiene problemas para habilitar DKIM para su dominio personalizado, siga estos pasos:

- La mayoría de los problemas de configuración de DKIM están relacionados con registros DNS incorrectos. Compruebe que el registro DKIM CNAME **(no** un registro TXT) tiene el formato correcto. Para obtener más información, vea este [tema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Después de crear o actualizar los registros DNS DKIM en el servicio de hospedaje DNS del dominio (normalmente, el registrador de dominios), espere a que se propaguen los registros DNS.

- Si no puede crear los registros DNS DKIM en el Centro de administración, puede reemplazar con su dominio personalizado (por ejemplo, contoso.com) y ejecutar este comando en \<CustomDomain\> [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
