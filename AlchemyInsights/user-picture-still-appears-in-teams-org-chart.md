---
title: La imagen de usuario sigue apareciendo en el organigrama de Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334410"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>La imagen de usuario sigue apareciendo en el organigrama de Microsoft Teams

Si se ha deshabilitado o quitado a una o varias personas de la organización y su foto de perfil aún aparece en el organigrama, es posible que la configuración **ShowInAddressLists** esté establecida en False: 

1. Vaya al Centro de administración de Microsoft 365 > [Usuarios activos](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) y seleccione al usuario cuya foto se sigue mostrando. 
1. Seleccione la pestaña **Correo** y asegúrese de que **Mostrar en la lista global de direcciones** está establecido en **No**.

Si el establecer **ShowInAddressLists** en **No** no funciona, compruebe lo siguiente: 

- Es posible que el usuario se muestre en la lista de destinatarios de Exchange. Para más información, consulte [Administrar listas de direcciones en Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Es posible que el usuario se muestre en la lista de direcciones de Azure Active Directory. Para obtener más información, consulte [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 