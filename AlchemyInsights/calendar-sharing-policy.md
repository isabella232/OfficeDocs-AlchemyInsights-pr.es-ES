---
title: Directiva de uso compartido de calendario 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091626"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Error de directiva al compartir un calendario

1. Realice una de las siguientes acciones, según corresponda para su situación:
    - Conectar para Exchange Online mediante PowerShell remoto. Para obtener más información, [vea Conectar para Exchange Online con PowerShell remoto](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - En el servidor local, abra el Shell Exchange administración.
2. Determine la directiva de uso compartido asignada al usuario. Para ello, ejecute el siguiente comando y anote la directiva devuelta:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Actualice la directiva de uso compartido para el usuario. Para ello, siga estos pasos:
    - Abra el Centro de administración de Exchange.
    - Haga **clic en** Organización y, a continuación, haga doble clic en la directiva asignada al usuario en Uso compartido **individual**. Esta es la directiva que se devolvió en el paso 2.
    - En la página Regla de uso compartido, seleccione el nivel de uso compartido de calendario que desea permitir en **Especificar qué información desea compartir;** haga clic **en Guardar**.

Para obtener más información, vea el [error "La](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)directiva no permite conceder permisos en este nivel a uno o varios de los destinatarios" cuando el usuario intenta compartir el calendario .
