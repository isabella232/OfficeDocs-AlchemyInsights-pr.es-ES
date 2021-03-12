---
title: Buscar y eliminar mensajes de correo electrónico en la organización
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737699"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Buscar y eliminar mensajes de correo electrónico en la organización

Siga estos pasos:

1. Si no es un administrador global, para buscar mensajes, su  cuenta debe agregarse al grupo de roles administrador de exhibición de documentos electrónicos o al rol de administración **Búsqueda de cumplimiento**. Para eliminar mensajes, deberá unirse al grupo de roles **Administración** de la organización o al rol **de administración Buscar y purgar**. Los permisos para estos roles se asignan en el [Centro de seguridad & cumplimiento.](https://protection.office.com)
2. [Cree una búsqueda de contenido](https://docs.microsoft.com/office365/securitycompliance/content-search) para buscar el mensaje que desea eliminar.
3. [Conéctese al Centro de seguridad y cumplimiento de PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Si usa MFA, consulte estas instrucciones: Conectarse a PowerShell del Centro de [seguridad & cumplimiento mediante la autenticación multifactor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Eliminar el mensaje: ejecute el `New-ComplianceSearchAction` cmdlet para eliminar el mensaje. Los mensajes eliminados se mueven a la carpeta Elementos recuperables de un usuario. Para obtener un comando de ejemplo, vea [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
