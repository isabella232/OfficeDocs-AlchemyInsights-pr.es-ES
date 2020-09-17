---
title: Teams permite o deshabilita el vídeo IP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670201"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams permite o deshabilita el vídeo IP

**Cambiar o crear una directiva de reunión**

Para cambiar o crear una directiva de reuniones, vaya al **Centro de administración de Microsoft Teams > Reuniones > Directivas de reuniones**. Seleccione una directiva de la lista o haga clic en **Agregar**. Si va a crear una nueva directiva, agregue un nombre y una descripción. El nombre no puede contener caracteres especiales ni tener más de 64 caracteres. Elija la configuración y, después, haga clic en **Guardar**.

Por ejemplo, supongamos que tiene muchos usuarios y quiere limitar el ancho de banda que necesitaría la reunión. Cree una nueva directiva personalizada denominada "ancho de banda limitado" y deshabilite las opciones siguientes:

En **Audio y vídeo**:

- Desactive Permitir la grabación en la nube.
- Desactive Permitir vídeo IP.

Luego asigne la directiva a los usuarios:

**Asignar una directiva de reunión a los usuarios**

1. En el panel de navegación izquierdo del Centro de administración de Microsoft Teams, vaya a **Usuarios** y, después, haga clic en el usuario.
2. Para seleccionar el usuario, haga clic a la izquierda del nombre de usuario y, después, en **Editar configuración**.
3. En **Directiva de reunión**, seleccione la directiva que quiera asignar y haga clic en **Aplicar**.

Para más información, consulte [Administrar directivas de reunión en Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
