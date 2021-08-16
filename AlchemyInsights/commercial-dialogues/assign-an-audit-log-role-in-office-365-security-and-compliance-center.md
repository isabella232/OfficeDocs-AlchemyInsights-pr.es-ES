---
title: Asignar un rol de registro de auditoría en el Centro de seguridad y cumplimiento de Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 5ddfda8687fe3ae2467ad221c7c083f46239826e23b10b91732ea06fd4649f3e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006187"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Asignar un rol de registro de auditoría en el Centro de seguridad y cumplimiento de Office 365

Para buscar el registro de auditoría de Office 365, un administrador debe tener asignado el rol de **Registros de auditoría de solo vista** o el rol de **Registros de auditoría** en Exchange Online. Estos roles se asignan a los grupos de roles de Administración de la organización y Administración de cumplimiento de forma predeterminada. Los administradores globales de Office 365 y Microsoft 365 pasan automáticamente a ser miembros del grupo de roles de Administración de la organización.

Para permitir a un usuario buscar con el mínimo nivel de privilegios, cree un grupo de roles personalizado en Exchange Online, agregue el rol de **Registros de auditoría de solo vista** o **Registros de auditoría** y, después, agregue el usuario como miembro del nuevo grupo de roles.

Para obtener más información, vea [Administrar grupos de roles en Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) y [Buscar el registro de auditoría del Centro de seguridad y cumplimiento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).