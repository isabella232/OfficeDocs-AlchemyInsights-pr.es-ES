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
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510143"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="a35bf-102">Asignar un rol de registro de auditoría en el Centro de seguridad y cumplimiento de Office 365</span><span class="sxs-lookup"><span data-stu-id="a35bf-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="a35bf-103">Para buscar el registro de auditoría de Office 365, un administrador debe tener asignado el rol de **Registros de auditoría de solo vista** o el rol de **Registros de auditoría** en Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a35bf-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="a35bf-104">Estos roles se asignan a los grupos de roles de Administración de la organización y Administración de cumplimiento de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="a35bf-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="a35bf-105">Los administradores globales de Office 365 y Microsoft 365 pasan automáticamente a ser miembros del grupo de roles de Administración de la organización.</span><span class="sxs-lookup"><span data-stu-id="a35bf-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="a35bf-106">Para permitir a un usuario buscar con el mínimo nivel de privilegios, cree un grupo de roles personalizado en Exchange Online, agregue el rol de **Registros de auditoría de solo vista** o **Registros de auditoría** y, después, agregue el usuario como miembro del nuevo grupo de roles.</span><span class="sxs-lookup"><span data-stu-id="a35bf-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="a35bf-107">Para obtener más información, vea [Administrar grupos de roles en Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) y [Buscar el registro de auditoría del Centro de seguridad y cumplimiento](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="a35bf-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>