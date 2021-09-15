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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327831"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Los informes de Centro de administración de Microsoft 365 no muestran el nombre de usuario legible

Los informes de Centro de administración de Microsoft 365 no muestran nombres de usuario, sino valores alfanuméricos, como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este es el comportamiento esperado y se ha comunicado en el Centro de mensajes (MC275344, publicado el 3 de agosto de 2021). 

Los administradores globales pueden revertir este cambio para su espacio empresarial y mostrar información de usuario identificable si las prácticas de privacidad de su organización lo permiten. Para revertir el cambio para el espacio empresarial:

1. En el centro de administración, vaya a **Configuración** > **Configuración de la organización** > [**Servicios**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )y seleccione **Informes**. 
1. En **Elija cómo mostrar la información de usuario**, seleccione **Mostrar información de usuario identificable en informes** y, a continuación, vuelva a ejecutar el informe.