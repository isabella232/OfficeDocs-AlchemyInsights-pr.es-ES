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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314221"
---
# <a name="active-directory-not-syncing"></a>Active Directory no se sincroniza

Si recibe errores de sincronización, como "no hay sincronización reciente" o observa el estado de sincronización de directorios en el portal de administración de Office, dice: "La última sincronización hace más de 3 días", puede ser que AADConnect tenga una configuración incorrecta o permisos insuficientes para realizar una sincronización.  

La reinstalación de AADConnect mediante la configuración rápida podría resolver el problema rápidamente:

1. [Descargue la versión más reciente de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga las instrucciones para la instalación rápida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect tiene que instalarse en Windows Server 2012 o posterior. Este servidor debe estar unido a un dominio y puede ser un controlador de dominio o un servidor miembro. Para obtener una lista completa de requisitos Conectar y requisitos previos de Azure AD, consulte [Prerequisites for Azure AD Conectar](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Para obtener más información sobre las cuentas de servicio de AADConnect, consulte [Azure AD Connect: Cuentas y permisos](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
