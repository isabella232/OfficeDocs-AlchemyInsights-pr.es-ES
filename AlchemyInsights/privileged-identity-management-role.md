---
title: Privileged Identity Management rol
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973246"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Los permisos no se conceden después de activar un rol**

Al activar un rol en Azure AD Privileged Identity Management (PIM), es posible que la activación no se propague al instante a todos los portales que requieren el rol con privilegios. A veces, incluso si el cambio se propaga, el almacenamiento en caché web en un portal puede provocar que el cambio no suba de inmediato.

Si la activación se retrasa, siga estos pasos:

1. Salga de Azure Portal y vuelva a iniciar sesión. Al activar un rol de Azure AD o un rol de recurso de Azure, verá las fases de la activación. Una vez completadas todas las fases, verá un vínculo "Cerrar sesión". Puede usar este vínculo para cerrar sesión. Esto resolverá la mayoría de los casos de retraso de activación.
2. En PIM, compruebe que aparece como miembro del rol.
3. Si está activando el rol Exchange administrador, asegúrese de cerrar sesión y volver a iniciar sesión. Si el problema persiste, abra un vale de soporte técnico y elirá esto como un problema. Si usa su rol de administrador Exchange para tener acceso al Centro de seguridad y cumplimiento, consulte el siguiente paso.
4. Si está activando un rol para tener acceso al Centro de seguridad y cumplimiento o si está activando el rol de administrador de SharePoint, experimentará algún retraso de activación de unos minutos hasta unas pocas horas. Este es un problema conocido y estamos trabajando activamente con estos equipos para resolver este problema tan pronto como sea posible.

Para obtener más información, vea:

- [Activar mis roles de Azure AD en PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activar mis roles de recursos de Azure en PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Los permisos no se quitan después de desactivar un rol o de que la activación del rol expire.**

Cuando desactiva un rol en Azure AD Privileged Identity Management o cuando expira un período de activación de roles, puede haber un retraso en el que siga teniendo acceso.

Si la desactivación se retrasa, siga estos pasos:

1. Si está desactivando el rol de administrador de Exchange o el período de activación del rol expira y observa un retraso significativo antes de quitar los permisos, abra un vale de soporte técnico e informe al ingeniero de soporte técnico para que le ayude a presentar un vale con el equipo de Administración de acceso privilegiado (PAM) dentro de Office sobre este problema.
2. Si el período de activación ha expirado, pero aún tiene la sesión del explorador abierta, cierre el explorador. Puede seguir usando el rol hasta que cierre esa sesión. Este es un problema conocido y estamos viendo una posible corrección para revocar activamente cada sesión una vez que la activación ha expirado.

Si el retraso es diferente de estos dos escenarios, abra un vale de soporte técnico.
