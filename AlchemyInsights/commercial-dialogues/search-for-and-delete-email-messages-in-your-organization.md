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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948900"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Buscar y eliminar mensajes de correo electrónico en la organización

Siga estos pasos:

1. Si no es un administrador global, para buscar mensajes, su  cuenta debe agregarse al grupo de roles administrador de exhibición de documentos electrónicos o al rol de administración **Búsqueda de cumplimiento**. Para eliminar mensajes, deberá unirse al grupo de roles **Administración** de la organización o al rol **de administración Buscar y purgar**. Los permisos para estos roles se asignan en el [Centro de seguridad & cumplimiento.](https://protection.office.com)
2. [Cree una búsqueda de contenido](https://docs.microsoft.com/office365/securitycompliance/content-search) para buscar el mensaje que desea eliminar.
3. [Conectarse a PowerShell del Centro de seguridad y cumplimiento](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Si usa MFA, vea estas instrucciones: Conectar [PowerShell del](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) Centro de seguridad & cumplimiento con la autenticación multifactor
4. Eliminar el mensaje: ejecute el `New-ComplianceSearchAction` cmdlet para eliminar el mensaje. Los mensajes eliminados se mueven a la carpeta Elementos recuperables de un usuario. Para obtener un comando de ejemplo, vea [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
