---
title: Error de dirección proxy al crear un buzón compartido
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062925"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Error de dirección de proxy al crear un buzón u otro objeto habilitado para correo electrónico

Si intentó crear un objeto habilitado para correo electrónico (buzón de correo, buzón compartido, etc.) y recibió el error "La dirección proxy "SMTP:alias@domain.com" ya se está utilizando...", la dirección de correo electrónico que eligió ya la toma otro objeto habilitado para correo electrónico de su organización.
  
Debe buscar el usuario, grupo, buzón compartido o carpeta pública que tiene esta dirección de correo electrónico y eliminarlo o cambiar su dirección de correo electrónico. A continuación, puede crear un nuevo objeto habilitado para correo electrónico con la dirección de correo electrónico liberada. Use La búsqueda en la página principal para encontrarlo. También puede usar el siguiente comando Exchange Online PowerShell para buscarlo:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Si no desea eliminar la dirección de correo electrónico existente, elija una nueva dirección de correo electrónico para el nuevo objeto que está creando.
  