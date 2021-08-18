---
title: Sincronización de contactos de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327350"
---
# <a name="teams-contacts-sync"></a>Sincronización de contactos de Teams

Teams utiliza tanto los contactos que tenga en el Active Directory de su organización como los que se hayan agregado a la carpeta predeterminada de Outlook del usuario. Si no puede ver los contactos en Microsoft Teams, pruebe lo siguiente:

**Nota:** Si la información de uno o varios contactos se ha actualizado recientemente, puede que los contactos tarden hasta 48 horas en sincronizarse.

1. Cierre la sesión de Teams y reinicie. Compruebe si ya se muestran los contactos.
1. Borre la caché de Teams:
    1. Vaya a **%appdata%\Microsoft\Teams**.
    1. Elimine el contenido de la carpeta.
    1. Reinicie el equipo e inicie Teams.
1. Si el contacto está en Outlook, asegúrese de agregarlo a la lista de contactos. En Outlook, en la barra de direcciones, seleccione **Archivo** y, a continuación, seleccione **Agregar a contactos**.
1. Asegúrese de que el buzón de Exchange del usuario está hospedado en línea (no localmente). Para obtener más información, vea [Interacción entre Exchange y Microsoft Teams](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
1. Asegúrese de haber agregado el número de teléfono del contacto a la información de contacto.
1. Busque la dirección de correo electrónico del contacto en la barra de Búsqueda. Los contactos que recupere se sincronizarán con la lista de contactos.
