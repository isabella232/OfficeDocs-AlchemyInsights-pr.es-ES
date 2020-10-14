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
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451386"
---
# <a name="sendas-mail-enabled-public-folder"></a>Carpeta pública habilitada para correo enviar como

En el siguiente ejemplo se asignan los permisos "enviar como" para la carpeta pública habilitada para correo NewPF1 al usuario Jason.

Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights ' sendas '

Para obtener información detallada acerca de la sintaxis y los parámetros, consulte [asignar los permisos "enviar como" o "enviar en nombre de" para las carpetas públicas habilitadas para correo](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

