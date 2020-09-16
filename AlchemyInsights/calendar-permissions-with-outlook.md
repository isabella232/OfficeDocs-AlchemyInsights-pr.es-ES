---
title: Permisos de calendario
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748810"
---
# <a name="calendar-permissions"></a>Permisos de calendario

Los usuarios pueden cambiar sus propios permisos de calendario con Outlook en la web u otros clientes, pero como administrador puede que también necesite investigar.  
Con el cmdlet de PowerShell de Exchange se mostrará el permiso en el calendario de un usuario:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para ver más información, consulte lo siguiente:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Los permisos de calendario se usan en el uso compartido de calendarios, para ver más información sobre cómo compartir un calendario de Outlook, consulte estos artículos:

- [Compartir un calendario de Outlook con otras personas](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Compartir el calendario en Outlook en la web para la empresa](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para solucionar problemas del permiso de calendario, puede usar la herramienta [Asistente para soporte y recuperación](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .