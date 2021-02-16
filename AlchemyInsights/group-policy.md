---
title: Directiva de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243921"
---
# <a name="group-policy"></a>Directiva de grupo

La configuración de los objetos de usuario y equipo en Azure Active Directory Domain Services (Azure AD DS) suele administrarse con objetos de directiva de grupo (GPO). Azure AD DS incluye GPO integrados para los usuarios de AADDC y los contenedores de equipos AADDC. Puede personalizar estos GPO integrados para configurar las directivas de grupo según sea necesario para su entorno. Los miembros del grupo de administradores de Azure AD DC tienen privilegios de administración de directivas de grupo en el dominio de Azure AD DS y también pueden crear GPO personalizados y unidades organizativas (OU). Para obtener más información sobre qué es una directiva de grupo y cómo funciona, consulte la [Información general de la directiva de grupo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

En un entorno híbrido, las directivas de grupo configuradas en un entorno local de AD DS no se sincronizan con Azure AD DS. Para definir opciones de configuración para usuarios o equipos en Azure AD DS, edite uno de los GPO predeterminados o cree uno personalizado.

El artículo [Administrar directiva de grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) le muestra cómo instalar las Herramientas de administración de directivas de grupo, editar los GPO integrados y crear GPO personalizados.



