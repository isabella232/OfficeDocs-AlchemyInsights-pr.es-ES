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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822868"
---
# <a name="active-directory-not-syncing"></a>Active Directory no se sincroniza

Si recibe errores de sincronización, como "no hay sincronización reciente" o observa el estado de sincronización de directorios en el portal de administración de Office, dice: "La última sincronización hace más de 3 días", puede ser que AADConnect tenga una configuración incorrecta o permisos insuficientes para realizar una sincronización.  

La reinstalación de AADConnect mediante la configuración rápida puede resolver el problema rápidamente:

1. [Descargue la versión más reciente de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga las instrucciones para la instalación rápida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para obtener más información sobre las cuentas de servicio de AADConnect, consulte [Azure AD Connect: Cuentas y permisos](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
