---
title: Modificar Microsoft Edge mediante variables de directorio de datos en lugar de rutas de acceso codificadas de forma rígida
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113433"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modificar Microsoft Edge mediante variables de directorio de datos en lugar de rutas de acceso codificadas de forma rígida

Por ejemplo, en Windows, para almacenar los datos de perfil en los datos de la aplicación local de un usuario, en lugar de la ubicación predeterminada, establezca la directiva **UserDataDir** en **${local_app_data}\Edge\Profile**. 

Para obtener más información, vea [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).