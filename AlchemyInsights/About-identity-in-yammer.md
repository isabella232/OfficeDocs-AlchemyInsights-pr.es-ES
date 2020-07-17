---
title: Acerca de la identidad en Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146806"
---
# <a name="about-identity-in-yammer"></a>Acerca de la identidad en Yammer

Se recomienda que todas las redes realicen los siguientes pasos para evitar problemas relacionados con la identidad:

1. Exigir la identidad de Office 365 después de aprovisionar cuentas de Microsoft 365 para los usuarios en Azure AD con objeto de garantizar que todos los usuarios inicien sesión con su cuenta de Microsoft 365 principal. Para obtener más información, vea [Exigir la identidad de Office 365 para usuarios de Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Consolidar varias redes de Yammer. Las configuraciones heredadas de Yammer permite conectar varias redes de Yammer a un espacio empresarial. Para obtener más información, vea [Migración de red: consolidar varias redes de Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Si lo desea, puede exigir licencias de Yammer para bloquear a los usuarios de Yammer en caso de que no tengan una licencia. Para obtener más información, vea [Administrar licencias de usuario de Yammer en Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Por último, auditar la lista de usuarios de las redes antiguas de Yammer y suspender a los usuarios antiguos. Se recomienda que suspenda (desactive) a los usuarios en lugar de eliminarlos, ya que la eliminación es irreversible. Para obtener más información, vea [Auditar usuarios de Yammer en redes conectadas a Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) y [Eliminar usuarios](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Si configura Yammer siguiendo estos pasos, también estará listo para configurar la red de Yammer para el modo nativo de Microsoft 365. Para obtener más información, vea [Configurar su red de Yammer para el Modo nativo para Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).