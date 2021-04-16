---
title: Desuso de Exchange PowerShell y autenticación básica
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813489"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Desuso de Exchange PowerShell y autenticación básica

Para obtener la información más reciente sobre cómo conectarse a Exchange Online PowerShell sin usar autenticación básica, [vaya aquí](https://aka.ms/exops-docs). El módulo PowerShell V2 no usa la autenticación básica.

Tenga en cuenta que la Autenticación básica debe estar habilitada en el equipo cliente.
El nuevo módulo PowerShell V2 usa la Autenticación moderna para establecer la conexión con el fin de habilitar todos los cmdlets V2 basados en REST. Además de los cmdlets V2, también le permite tener acceso a cmdlets antiguos remotos de PowerShell (RPS), lo que requiere que se establezca una sesión de PowerShell remota. Establecer una sesión de RPS en un equipo con Windows requiere que se habilite la Autenticación básica WinRM en el equipo cliente aunque el módulo use un mecanismo de autenticación moderno para autenticarse en el servicio. La canalización de autenticación básica de WinRM se usa para transportar los tokens de autenticación modernos. Si la Autenticación básica WinRM está deshabilitada en el equipo cliente, los nuevos cmdlets V2 seguirán funcionando (pero los cmdlets de RPS antiguos no se mostrarán).
