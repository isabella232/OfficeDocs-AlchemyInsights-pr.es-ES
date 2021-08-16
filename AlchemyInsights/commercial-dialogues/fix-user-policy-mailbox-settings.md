---
title: Corregir la configuración de la directiva de usuario/buzón de correo
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034735"
---
# <a name="fix-user-policymailbox-settings"></a>Corregir la configuración de la directiva de usuario/buzón de correo

La configuración del correo no deseado en el buzón afectó a este mensaje. Para revisar la configuración, haga lo siguiente:

1. Inicie Exchange Shell de administración. Para obtener más información, vea [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Ejecute este comando (mediante la dirección de correo electrónico del usuario):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Compruebe si la dirección de correo electrónico del remitente forma parte de **TrustedSendersAndDomains** o **BlockedSendersAndDomains**. Si la dirección de correo electrónico está en una de las listas, es posible que tenga que quitarla. Para obtener más información, [vea Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
