---
title: Asignar grupos a un rol de Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036257"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Asignar grupos a un rol de Azure AD

Para asignar un grupo de Azure AD con origen de autoridad en Azure AD a un rol de Azure AD, siga los siguientes pasos:

1. Crear grupo - Para crear un grupo nuevo:

    a. Inicie sesión en el Centro de administración de Azure AD con los permisos de **rol de administración con privilegios** o de **administrador global**.
    b. Seleccione **Azure Active Directory > Grupos > Todos los grupos > Nuevo grupo**.
    c. Cree el grupo.

2. Puede asignar el rol al grupo durante la creación del grupo o después de crearlo.

    a. Para asignar un rol al grupo en el momento de crearlo, cambie el botón de alternancia a **Los roles de Azure AD se pueden asignar al grupo** y cree el grupo.
    b. Para asignar un rol al grupo después de creado, vaya a la pestaña **Roles asignados** del grupo recién creado y asigne el rol al grupo.  

**Administrar la suscripción a un grupo asignado al rol de Azure AD**

Para evitar la elevación de privilegios, de forma predeterminada, solo los administradores de roles con privilegios y los administradores globales pueden modificar la pertenencia a un grupo que esté asignado a un rol. En cambio, puede asignar un propietario a este grupo y delegar esta tarea.

Para obtener más información sobre cómo asignar grupos en la nube a roles de Azure AD, vea [Asignar roles de AD a grupos en la nube](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Para obtener más información sobre cómo solucionar problemas de roles asignados a grupos en la nube, vea [Solución de problemas de roles asignados a grupos en la nube](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





