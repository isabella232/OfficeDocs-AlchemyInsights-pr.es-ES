---
title: La imagen de usuario no se muestra en el organigrama de Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467393"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>La imagen de usuario no se muestra en el organigrama de Microsoft Teams

Si a una o más personas de su organización les falta la foto de perfil en el organigrama, es posible que la configuración **ShowInAddressLists** esté establecida en **Falsa**:

1. Vaya al Centro de administración de Microsoft 365 > [**Usuarios activos**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) y seleccione al usuario al que le falta la foto. 
1. Seleccione la pestaña **Correo** y asegúrese de que **Mostrar en la lista global de direcciones** está establecido en **Sí**. 

Si establecer **ShowInAddressLists** en **Sí** no funciona, compruebe lo siguiente:

- Es posible que el usuario esté oculto en la lista de destinatarios de Exchange. Para obtener más información, consulte [Administrar listas de direcciones en Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Es posible que el usuario esté oculto en la lista de direcciones de Azure Active Directory. Para obtener más información, consulte [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
