---
title: Modifique Microsoft Edge usando variables de directorio de datos en lugar de rutas codificadas de forma rígida
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992308"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modifique Microsoft Edge usando variables de directorio de datos en lugar de rutas codificadas de forma rígida

Por ejemplo, en Windows, para almacenar los datos de perfil en los datos de la aplicación local de un usuario, en lugar de la ubicación predeterminada, establezca la directiva *UserDataDir* en **${local_app_data}\Edge\Profile**.

Para obtener más información, consulte [Crear variables de directorio de datos de usuario de Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).