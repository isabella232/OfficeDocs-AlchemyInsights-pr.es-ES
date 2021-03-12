---
title: Mover automáticamente mensajes de correo electrónico al buzón de archivo
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737587"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Mover automáticamente mensajes de correo electrónico al buzón de archivo

Este es el modo de configurar una directiva para mover automáticamente el correo electrónico antiguo de un usuario al buzón de archivo:

1. Vaya a [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data governance Archive para comprobar que se ha habilitado un buzón de archivo para el  >    >   usuario. Si no lo ha hecho, haga clic **en Habilitar** **y,** a continuación, en Sí en el cuadro de advertencia.
2. Vaya al [**Centro de administración de Exchange > administración de cumplimiento > etiquetas de retención**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Elija el icono + y, a **continuación, elija aplicar automáticamente a todo el buzón**.
4. Asigne un nombre a la etiqueta de retención y elija **Mover a Archivo**. Para el período de retención, escriba el tiempo que desee, como 90 días. Haga clic en **Guardar**.
5. Ahora cree una directiva de retención: elija **directivas de retención,** elija el icono para agregar una nueva directiva.
6. Asigne un nombre a la directiva de retención y, a continuación, haga clic y desplácese para buscar y agregar la etiqueta de retención que acaba de crear. Haga clic en **Guardar**.
7. Por último, aplique la directiva de retención al buzón del usuario: aún en el Centro de administración de Exchange, vaya a **buzones**  >  **de destinatarios**. Elija todos los usuarios a los que desea aplicar la directiva y, a continuación, **elija Editar** (icono de lápiz).
8. En el cuadro de diálogo, haga clic **en Características del buzón**. En **Directiva de retención,** aplique la directiva que acaba de crear > **Guardar**.
9. Para obtener instrucciones para aplicar la directiva a todos los usuarios, vea [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
