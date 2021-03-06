---
title: Establecer ClientAccessServerEnabled en True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510002"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Establecer ClientAccessServerEnabled en True

Si no puede abrir un mensaje de correo electrónico cifrado y, en su lugar, ver los datos **adjuntos de rpmsg,** siga estos pasos:

1. Conéctese a Exchange Online PowerShell.

> [!NOTE]
> Para conectarse a Exchange Online PowerShell, debe iniciar sesión con un administrador global o una cuenta de administrador de Exchange.

   a. Abra Windows PowerShell y, a continuación, ejecute el siguiente comando: `$UserCredential = Get-Credential`
b. En el Windows PowerShell de diálogo Solicitud de **credencial,** escriba su cuenta y contraseña de trabajo o escuela, c. Haga clic en **Aceptar**. 

2. Ejecute el siguiente comando para crear una nueva sesión:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Ejecute el siguiente comando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Ejecutar `Get-IRMConfiguration` comando.

4. Compruebe la **configuración ClientAccessServerEnabled.** 

    a. Si **la configuración clientAccessServerEnabled** está establecida en **False,** ejecute el siguiente cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Cierre siempre la sesión de PowerShell con el siguiente comando: `Remove-PSSession $Session`

Para obtener más información, [vea Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

