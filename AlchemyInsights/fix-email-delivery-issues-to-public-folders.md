---
title: Corregir problemas de entrega de correo electrónico en carpetas públicas habilitadas para correo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068829"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corregir problemas de entrega de correo electrónico en carpetas públicas habilitadas para correo

Si los remitentes externos no pueden enviar mensajes a las carpetas públicas habilitadas para correo y los remitentes reciben el error: no se pudo encontrar **(550 5.4.1),** compruebe que el dominio de correo electrónico de la carpeta pública esté configurado como un dominio de retransmisión interno en lugar de un dominio autoritativo:

1. Abra el [Exchange de administración (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Vaya a **Flujo de correo** Dominios \> **aceptados,** seleccione el dominio aceptado y, a continuación, haga clic en **Editar**.

3. En la página de propiedades que se abre, si el tipo de dominio está establecido en **Autoritativo,** cambie el valor a **Retransmisión** interna y, a continuación, haga clic en **Guardar**.

Si los remitentes externos reciben el error no tiene permiso **(550 5.7.13),** ejecute el siguiente comando en [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver los permisos para usuarios anónimos en la carpeta pública:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Por ejemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Para permitir que los usuarios externos envíen correo electrónico a esta carpeta pública, agregue el derecho de acceso CreateItems al usuario Anónimo. Por ejemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
