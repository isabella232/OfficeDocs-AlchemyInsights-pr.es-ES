---
title: Rol de administración de identidades con privilegios
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086377"
---
# <a name="privileged-identity-managementpim-role"></a>Rol de administración de identidades privilegiada (PIM)

**No se conceden permisos tras activar un rol**

Al activar un rol en Azure AD privileged Identity Management (PIM), es posible que la activación no se propague inmediatamente a todos los portales que requieran el rol privilegiado. A veces, incluso si se propaga el cambio, el almacenamiento en caché de Web en un portal puede hacer que el cambio no surta efecto inmediatamente.

Si la activación se retrasa, siga estos pasos:

1. Cierre la sesión de Azure portal y, a continuación, vuelva a iniciar sesión. Al activar un rol de Azure AD o un rol de recurso de Azure, verá las fases de la activación. Una vez completadas todas las etapas, verá el vínculo "cerrar sesión". Puede usar este vínculo para cerrar la sesión. Esto resolverá la mayoría de los casos para el retraso de la activación.
2. En PIM, compruebe que se encuentra como miembro de la función.
3. Si está activando el rol de administrador de Exchange, asegúrese de cerrar la sesión y volver a iniciarla. Si el problema persiste, abra una incidencia de soporte técnico y provoque esto como un problema. Si usa el rol de administrador de Exchange para tener acceso al centro de seguridad y cumplimiento, consulte el paso siguiente.
4. Si está activando un rol para obtener acceso al centro de seguridad y cumplimiento o si está activando el rol de administrador de SharePoint, experimentará algunos retrasos en la activación desde hace unos minutos, hasta unas horas. Se trata de un problema conocido y estamos trabajando activamente con estos equipos para resolver este problema tan pronto como sea posible.

Para más información, vea:

- [Activar mis roles de Azure AD en PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Activar mis roles de recursos de Azure en PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Los permisos no se quitan después de desactivar una función o la activación de la función expira**

Cuando se desactiva un rol en la administración de identidades privilegiada de Azure AD o cuando expira un período de activación de rol, es posible que se produzca un retraso en el que continúe teniendo acceso.

Si la desactivación se retrasa, siga estos pasos:

1. Si está desactivando el rol de administrador de Exchange o el período de activación de roles expira y observa un retraso significativo antes de que se quiten los permisos, abra un vale de soporte técnico y dígale a su ingeniero de soporte técnico que le ayude a archivar un vale con el equipo de administración de acceso privilegiado (PAM) en Office sobre este problema.
2. Si ha expirado el período de activación, pero todavía tiene la sesión del explorador abierta, cierre el explorador. Puede seguir usando el rol hasta que cierre esa sesión. Se trata de un problema conocido y estamos examinando una solución potencial para revocar activamente cada sesión una vez que la activación haya expirado.

Si el retraso es distinto de estos dos escenarios, abra una incidencia de soporte técnico.
