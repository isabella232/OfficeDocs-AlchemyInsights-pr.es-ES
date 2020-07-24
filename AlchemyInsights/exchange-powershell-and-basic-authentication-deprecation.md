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
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="4a4a4-102">Desuso de Exchange PowerShell y autenticación básica</span><span class="sxs-lookup"><span data-stu-id="4a4a4-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="4a4a4-103">Para obtener la información más reciente sobre cómo conectarse a Exchange Online PowerShell sin usar autenticación básica, [vaya aquí](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="4a4a4-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="4a4a4-104">El módulo PowerShell V2 no usa la autenticación básica.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="4a4a4-105">Tenga en cuenta que la Autenticación básica debe estar habilitada en el equipo cliente.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="4a4a4-106">El nuevo módulo PowerShell V2 usa la Autenticación moderna para establecer la conexión con el fin de habilitar todos los cmdlets V2 basados en REST.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="4a4a4-107">Además de los cmdlets V2, también le permite tener acceso a cmdlets antiguos remotos de PowerShell (RPS), lo que requiere que se establezca una sesión de PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="4a4a4-108">Establecer una sesión de RPS en un equipo con Windows requiere que se habilite la Autenticación básica WinRM en el equipo cliente aunque el módulo use un mecanismo de autenticación moderno para autenticarse en el servicio.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="4a4a4-109">La canalización de autenticación básica de WinRM se usa para transportar los tokens de autenticación modernos.</span><span class="sxs-lookup"><span data-stu-id="4a4a4-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="4a4a4-110">Si la Autenticación básica WinRM está deshabilitada en el equipo cliente, los nuevos cmdlets V2 seguirán funcionando (pero los cmdlets de RPS antiguos no se mostrarán).</span><span class="sxs-lookup"><span data-stu-id="4a4a4-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
