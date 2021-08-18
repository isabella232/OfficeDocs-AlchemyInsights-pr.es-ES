---
title: Falta correo electrónico en cuarentena
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
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329679"
---
# <a name="missing-emails-in-quarantine"></a>Falta correo electrónico en cuarentena

Los administradores [pueden ver, liberar o eliminar estos mensajes](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

En el Microsoft 365 Defender en <https://security.microsoft.com> , vaya a **Revisar** \> **cuarentena**. O bien, para ir directamente a la **página Cuarentena,** use <https://security.microsoft.com/quarantine> .  

Para obtener más información acerca de los valores de búsqueda y filtro que puede usar, vea [Manage quarantined messages and files as an admin in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Los cmdlets que usa para ver y administrar mensajes y archivos en cuarentena son:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)tenga en cuenta que este cmdlet solo es para mensajes, no archivos de datos adjuntos de Caja fuerte para SharePoint, OneDrive o Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
