---
title: Varios objetos tienen la misma dirección de correo electrónico que la identidad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724632"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Varios objetos tienen la misma dirección de correo electrónico que la identidad

**Varios objetos**

Uno de los motivos comunes de este error es que no pueda redirigir correctamente una solicitud de Outlook Web Access en la presencia de varios objetos que tengan la misma dirección de correo electrónico que la identidad. Para encontrar estos objetos, ejecute los siguientes comandos:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Para resolver este problema, quite varios objetos con la misma identidad de correo electrónico y asegúrese de que existe un único objeto con la identidad de correo electrónico específica y de que su tipo de destinatario es UserMailbox.

**La misma dirección se usa para los buzones de cliente y empresa**

Otra causa es cuando se usa la misma dirección para los buzones de cliente y de empresa. En este caso, el usuario tendrá que cambiar el alias de consumidor principal hasta que cibercafé sea compatible con este escenario. Este es un error permanente que no desaparecerá sin intervención.

Para obtener más información, consulte [Cambiar la dirección de correo electrónico o el número de teléfono de la cuenta de Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).