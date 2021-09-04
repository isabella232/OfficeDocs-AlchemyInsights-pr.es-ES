---
title: Los informes de Centro de administración de Microsoft 365 no muestran el nombre de usuario legible
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896351"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Los informes de Centro de administración de Microsoft 365 no muestran el nombre de usuario legible

Los informes de Centro de administración de Microsoft 365 no muestran nombres de usuario, sino valores alfanuméricos, como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este es el comportamiento esperado y se ha comunicado en el Centro de mensajes (MC275344, publicado el 3 de agosto de 2021). 

Los administradores globales pueden revertir este cambio para su espacio empresarial y mostrar información de usuario identificable si las prácticas de privacidad de su organización lo permiten. Para revertir el cambio para el espacio empresarial:

1. En el centro de administración, vaya a **Configuración** > **Configuración de la organización** > [**Servicios**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)y seleccione **Informes**. 
1. En **Elija cómo mostrar la información de usuario**, seleccione **Mostrar información de usuario identificable en informes** y, a continuación, vuelva a ejecutar el informe.