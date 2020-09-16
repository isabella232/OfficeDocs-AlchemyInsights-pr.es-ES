---
title: Corregir problemas de configuración de DKIM
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744967"
---
# <a name="fix-dkim-setup-issues"></a>Corregir problemas de configuración de DKIM

Si experimenta problemas para habilitar DKIM para su dominio personalizado, siga estos pasos:

- La mayoría de los problemas de configuración de DKIM están relacionados con registros DNS incorrectos. Compruebe que el registro CNAME de DKIM (**no** un registro txt) tiene el formato correcto. Para obtener más información, vea este [tema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Después de crear o actualizar los registros DNS de DKIM en el servicio de hospedaje DNS para su dominio (normalmente, el registrador de dominios), espere a que se propaguen los registros DNS.

- Si no puede crear los registros DNS de DKIM en el centro de administración, puede reemplazarlos \<CustomDomain\> con el dominio personalizado (por ejemplo, contoso.com) y ejecutar este comando en [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
