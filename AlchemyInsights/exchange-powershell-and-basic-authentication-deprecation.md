---
title: Desuso de Exchange PowerShell y autenticación básica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205212"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Desuso de Exchange PowerShell y autenticación básica

Para obtener la información más reciente sobre cómo conectarse a Exchange Online PowerShell sin usar autenticación básica, [vaya aquí](https://aka.ms/exops-docs). El módulo PowerShell V2 no usa la autenticación básica.

Tenga en cuenta que la Autenticación básica debe estar habilitada en el equipo cliente.
El nuevo módulo PowerShell V2 usa la Autenticación moderna para establecer la conexión con el fin de habilitar todos los cmdlets V2 basados en REST. Además de los cmdlets V2, también le permite tener acceso a cmdlets antiguos remotos de PowerShell (RPS), lo que requiere que se establezca una sesión de PowerShell remota. Establecer una sesión de RPS en un equipo con Windows requiere que se habilite la Autenticación básica WinRM en el equipo cliente aunque el módulo use un mecanismo de autenticación moderno para autenticarse en el servicio. La canalización de autenticación básica de WinRM se usa para transportar los tokens de autenticación modernos. Si la Autenticación básica WinRM está deshabilitada en el equipo cliente, los nuevos cmdlets V2 seguirán funcionando (pero los cmdlets de RPS antiguos no se mostrarán).
