---
title: Implementación de GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067857"
---
# <a name="gpo-deployment"></a>Implementación de GPO

La configuración de los objetos de usuario y equipo en Azure Active Directory Domain Services (Azure AD DS) suele administrarse con objetos de directiva de grupo (GPO). Azure AD DS incluye GPO integrados para los usuarios de AADDC y los contenedores de equipos AADDC. Puede personalizar estos GPO integrados para configurar las directivas de grupo según sea necesario para su entorno. Los miembros del grupo de administradores de Azure AD DC tienen privilegios de administración de directivas de grupo en el dominio de Azure AD DS y también pueden crear GPO personalizados y unidades organizativas (OU). Para obtener más información sobre qué es la directiva de grupo y cómo funciona, vea [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

En un entorno híbrido, las directivas de grupo configuradas en un entorno local de AD DS no se sincronizan con Azure AD DS. Para definir opciones de configuración para usuarios o equipos en Azure AD DS, edite uno de los GPO predeterminados o cree uno personalizado.

El artículo [Administrar directiva de grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) le muestra cómo instalar las Herramientas de administración de directivas de grupo, editar los GPO integrados y crear GPO personalizados.
