---
title: Active Directory no se sincroniza
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930992"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="d68de-102">Active Directory no se sincroniza</span><span class="sxs-lookup"><span data-stu-id="d68de-102">Active Directory not syncing</span></span>

<span data-ttu-id="d68de-103">Si recibe errores de sincronización, como "no hay sincronización reciente" o observa el estado de sincronización de directorios en el portal de administración de Office, dice: "La última sincronización hace más de 3 días", puede ser que AADConnect tenga una configuración incorrecta o permisos insuficientes para realizar una sincronización.</span><span class="sxs-lookup"><span data-stu-id="d68de-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="d68de-104">La reinstalación de AADConnect mediante la configuración rápida podría resolver el problema rápidamente:</span><span class="sxs-lookup"><span data-stu-id="d68de-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="d68de-105">[Descargue la versión más reciente de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="d68de-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="d68de-106">[Siga las instrucciones para la instalación rápida](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="d68de-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="d68de-107">Azure AD Connect tiene que instalarse en Windows Server 2012 o posterior.</span><span class="sxs-lookup"><span data-stu-id="d68de-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="d68de-108">Este servidor debe estar unido a un dominio y puede ser un controlador de dominio o un servidor miembro.</span><span class="sxs-lookup"><span data-stu-id="d68de-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="d68de-109">Para obtener una lista completa de requisitos Conectar y requisitos previos de Azure AD, consulte [Prerequisites for Azure AD Conectar](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="d68de-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="d68de-110">Para obtener más información sobre las cuentas de servicio de AADConnect, consulte [Azure AD Connect: Cuentas y permisos](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="d68de-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
