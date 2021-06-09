---
title: Administrar el registro del seminario web
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798661"
---
# <a name="manage-webinar-registration"></a>Administrar el registro del seminario web

Puede administrar quién puede registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams. Para instalar PowerShell para Teams, consulte [PowerShell para Teams](/microsoftteams/teams-powershell-install). 

De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **Todos**. 

Si no ve la opción para permitir el registro para todos los usuarios en la invitación de reunión, vuelva a ejecutar la configuración *WhoCanRegister* para todos y espere 24 horas. Para volver a ejecutar *WhoCanRegister*, use el comando de PowerShell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Nota**: si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web. Para más información y para habilitar esta configuración, consulte [Administrar la configuración de la reunión en Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.

Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).
