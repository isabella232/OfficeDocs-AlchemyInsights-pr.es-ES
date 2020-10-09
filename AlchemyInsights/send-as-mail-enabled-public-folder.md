---
title: Enviar como carpeta pública habilitada para correo en EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394692"
---
# <a name="sendas-mail-enabled-public-folder"></a>Carpeta pública habilitada para correo enviar como

En el siguiente ejemplo se asignan los permisos "enviar como" para la carpeta pública habilitada para correo NewPF1 al usuario Jason.

Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' sendas '

Para obtener información detallada acerca de la sintaxis y los parámetros, consulte [asignar los permisos "enviar como" o "enviar en nombre de" para las carpetas públicas habilitadas para correo](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).
