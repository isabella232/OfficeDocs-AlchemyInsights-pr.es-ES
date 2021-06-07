---
title: Habilitar los seminarios web de Teams
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760858"
---
# <a name="enable-teams-webinars"></a>Habilitar los seminarios web de Teams

Los seminarios web están habilitados de forma predeterminada. Puede administrar quién puede programar y registrarse en los seminarios web de Teams mediante los comandos de PowerShell de Teams.

- Todos los usuarios que puedan crear una reunión también podrán crear una reunión de seminario web. Si quiere administrar quién puede programar los seminarios web de Teams, use *AllowMeetingRegistration*. 
- De forma predeterminada, *WhoCanRegister* está habilitado y establecido en **Todos**. Si desea desactivar el registro de la reunión, establezca *AllowMeetingRegistration* en **False**.

Para cambiar esta configuración, debe instalar [PowerShell de Teams](/microsoftteams/teams-powershell-install). Además, las directivas de la reunión aplican para los seminarios web de Teams. Por ejemplo, si la participación anónima está desactivada en la configuración de la reunión, los usuarios anónimos no podrán unirse a los seminarios web.

Para obtener más información sobre cómo configurar quién puede registrarse en los seminarios web, vea [Configurar quién puede registrarse en los seminarios web](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Para obtener más información sobre la configuración de las Listas Microsoft, consulte [Configuración de control para las Listas Microsoft](/sharepoint/control-lists).