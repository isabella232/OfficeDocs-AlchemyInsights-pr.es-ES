---
title: Solución de problemas de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716116"
---
# <a name="troubleshoot-group-issues"></a>Solución de problemas de grupo

**Necesito asignar un grupo a un rol de Azure AD**

Para asignar un grupo de Azure Active Directory (AD) a un rol de Azure AD, siga los siguientes pasos:

1. Crear grupo - Para crear un grupo nuevo:

    a. Inicie sesión en el Centro de administración de Azure AD con los permisos de rol de administración con privilegios o de administrador global. 
    b. Seleccione Azure Active Directory > Grupos > Todos los grupos > Nuevo grupo. 
    c. Cree el grupo.

2. Puede asignar el rol al grupo durante la creación del grupo o después de crearlo.

    a. Para asignar un rol al grupo en el momento de crearlo, cambie el botón de alternancia a Los roles de Azure AD se pueden asignar al grupo y cree el grupo.
    b. Para asignar un rol al grupo después de creado, vaya a la pestaña Roles asignados del grupo recién creado y asigne el rol al grupo.

**Necesito administrar la suscripción a un grupo asignado al rol de Azure AD**

1. Para evitar la elevación de privilegios, de forma predeterminada, solo los administradores de roles con privilegios y los administradores globales pueden modificar la pertenencia a un grupo que esté asignado a un rol. En cambio, puede asignar un propietario a este grupo y delegar esta tarea. Para más información, consulte [Uso de grupos en la nube para administrar asignaciones de roles en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Para preguntas comunes y consejos de solución de problemas para asignar roles a grupos en Azure AD, consulte [Solución de problemas relacionados con roles asignados a grupos en la nube](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Grupos dinámicos**

1. Si no encuentra los atributos integrados de usuario, asegúrese de que el atributo se encuentre en la lista de propiedades admitidas.
2. Si está buscando atributos integrados de dispositivo, asegúrese de que el atributo se encuentre en la lista de atributos de dispositivo. 
3. Además de los atributos integrados de usuario y de dispositivo, podría usar también los [Atributos de extensión](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Tras sincronizar los atributos de extensión de Windows Server AD en el entorno local o de una aplicación conectada de SaaS, los atributos deberían ser visibles en la lista desplegable del generador de reglas. El nombre personalizado de atributo se puede encontrar en el directorio mediante una consulta del atributo de usuario con PowerShell y con una búsqueda del nombre del atributo. Estos también se podrían usar al construir reglas en la sintaxis de regla.
4. Asegúrese de que su espacio empresarial tenga con la licencia adecuada. Los grupos dinámicos requieren que el espacio empresarial tenga una licencia premium Azure AD P1. Se puede acceder [aquí](https://azure.microsoft.com/pricing/details/active-directory/) a la lista de planes de licencia de Azure AD Se puede acceder [aquí](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing) a los planes de licencia de Enterprise Mobility + Security 
5. Asegúrese de que el rol del usuario que cree el grupo dinámico sea administrador global, administrador Intune, administrador de grupo o administrador de usuario.
6. Espere a que el grupo se rellene. En función del tamaño de su espacio empresarial, puede que el grupo tarde hasta 24 horas para rellenarse la primera vez tras un cambio de regla.
7. Para más información, consulte [Crear reglas basadas en atributos para la suscripción de grupos dinámicos](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Necesito eliminar un grupo**

1. Se pueden eliminar los grupos desde el directorio mediante el cmdlet Remove-AzureADGroup en el módulo de PowerShell de Azure AD.
2. Antes de intentar eliminar un grupo sincronizado en Azure AD, asegúrese de haber eliminado todas las licencias asignadas para evitar errores.
3. Para más información sobre la eliminación de grupos, consulte [Eliminar un grupo con una licencia asignada](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Necesito restaurar un grupo eliminado**

1. Si se elimina un grupo de Office 365, solo se puede restaurar hasta 30 días; después, tiene lugar la eliminación permanente. Una vez que se haya eliminado permanentemente, el grupo ya no podrá ser restaurado. Encontrará más información sobre cómo restaurar grupos [aquí](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Esta funcionalidad no se admite para grupos de seguridad y de distribución.
3. Asegúrese de tener autorización para restaurar un grupo de Office 365. Los administradores globales, administradores de grupo, administradores de cuentas de usuario, administradores de servicio de Intune, soporte técnico de nivel 1 o 2 para asociados y el propietario del grupo pueden restaurar un grupo.
4. Cuando un grupo dinámico se elimina y restaura, se ve como un grupo nuevo y se vuelve a rellenar según la regla. Es posible que este proceso tarde hasta 24 horas.
5. Para más información sobre cómo restaurar un grupo eliminado, consulte [Restaurar un grupo eliminado de Office 365 en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configuración de la política de caducidad de grupos**

1. Esta funcionalidad solo se admite para grupos de Office 365; no se admite para grupos de seguridad y de distribución.
2. Configurar y usar la directiva de expiración para grupos de Office 365 requiere una licencia de Azure AD Premium.
3. En estos momentos, solo se puede configurar una directiva de expiración para grupos de Office 365 en un espacio empresarial.
4. Solo los administradores globales, administradores de grupo, administradores de usuario y el propietario del grupo pueden renovar un grupo.
5. Si expira un grupo de Office 365, se elimina y solo se puede restaurar hasta 30 días; después, tiene lugar la eliminación permanente. Una vez que se haya eliminado permanentemente, el grupo ya no podrá ser restaurado. Encontrará más información sobre cómo restaurar grupos [aquí](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Renovación automática basada en la actividad**

Las actividades de usuario de SharePoint, Outlook y Teams puede desencadenar una renovación automática de grupo. Las actividades se comprueban a los 35 días, antes de que el grupo expire. Si hay actividad durante el actual ciclo de vida del grupo, el grupo será renovado automáticamente y no se enviará una notificación por correo electrónico a los propietarios del grupo.

**Intervalos de tiempo de notificación para grupos expirados**

1. Las notificaciones por correo electrónico se enviarán a los propietarios del grupo de Office 365 30 días, 15 días y 1 día antes de la expiración del grupo.
2. Cuando se configura la expiración por primera vez, cualquier grupo que sea más antiguo que el intervalo de expiración está configurado a 35 días hasta la expiración.
3. La fecha de expiración del grupo se calcula en función de la fecha de renovación del grupo, en lugar de la fecha de actualización de directiva. Si la directiva de expiración se actualiza, la fecha de expiración no cambiará.
4. Para más información, consulte [Directiva de expiración de grupo y correos electrónicos de renovación](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) y [Restaurar un grupo eliminado de Office 365 en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Permiso para crear un grupo**

Asegúrese de que está autorizado para crear un nuevo grupo. Los administradores globales pueden deshabilitar la creación de grupos en Azure Portal o el Panel de acceso. Puede que necesite que un administrador cree el nuevo grupo o que le conceda los permisos adecuados.

1. [Crear un nuevo grupo y agregar miembros en Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Crear grupos en PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Deshabilitar la creación de grupos en PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Administrar quién puede crear grupos de Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Deshabilitar la notificación de bienvenida de Office 365 mediante PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Roles administrativos de Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Administrar los permisos de creación de grupos**

1. Los administradores globales pueden administrar los permisos de creación de grupos para grupos de seguridad o de Office 365 creados en Azure Portal o el Panel de acceso. Para ello, configure las opciones **Los usuarios pueden crear grupos de seguridad en los portales de Azure** o **Los usuarios pueden crear grupo de Office 365 en los portales de Azure** en **Todos los grupos > General (Configuración)**.
2. Asimismo, puede restringir la creación de grupos y seleccionar un grupo de usuarios, si tiene una licencia Premium de Azure AD P1.

**Deshabilitar la notificación de bienvenida para nuevos miembros de un grupo de Office 365**

La notificación de bienvenida que se envía a los usuarios agregados a grupos de Office 365 puede ser deshabilitada si se establece `UnifiedGroupWelcomeMessageEnabled` en **Falso** en PowerShell. Obtenga información sobre esta configuración [aquí](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













