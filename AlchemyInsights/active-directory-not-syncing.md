---
title: Active Directory no se sincroniza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697646"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e70c4-102">Active Directory no se sincroniza</span><span class="sxs-lookup"><span data-stu-id="e70c4-102">Active Directory not syncing</span></span>

<span data-ttu-id="e70c4-103">Si recibe errores de sincronización, como "no hay sincronización reciente", o observa el estado de sincronización de directorios en el portal de administración de Office dice: "última sincronización hace más de 3 días", puede que los tiempos de usuario tengan una configuración incorrecta o permisos insuficientes para realizar una sincronización.</span><span class="sxs-lookup"><span data-stu-id="e70c4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e70c4-104">Si se reinstalan los valores de los-out mediante la configuración rápida, puede que se resuelva el problema rápidamente:</span><span class="sxs-lookup"><span data-stu-id="e70c4-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e70c4-105">[Descargue la versión más reciente de los](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="e70c4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e70c4-106">[Siga las instrucciones para la instalación rápida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e70c4-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e70c4-107">Para obtener más información sobre las cuentas de servicio de AADConnect, consulte [Azure AD Connect: Cuentas y permisos](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="e70c4-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
