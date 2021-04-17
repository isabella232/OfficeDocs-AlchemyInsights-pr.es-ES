---
title: Permisos de calendario
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819925"
---
# <a name="calendar-permissions"></a>Permisos de calendario

Los usuarios pueden cambiar sus propios permisos de calendario con Outlook en la Web u otros clientes, pero como administrador también es necesario investigar.  
Con el cmdlet de PowerShell de Exchange se mostrará el permiso en el calendario de un usuario:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Para obtener más información, vea lo siguiente:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Los permisos de calendario se usan en el uso compartido de calendarios, para ver más información sobre cómo compartir un calendario de Outlook, vea estos artículos:

- [Compartir un calendario de Outlook con otras personas](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Compartir el calendario en Outlook en la web para empresas](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Para solucionar problemas de permisos de calendario, puede usar la [herramienta Asistente para soporte](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) técnico y recuperación.