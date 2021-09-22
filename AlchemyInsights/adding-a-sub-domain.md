---
title: Agregar un subdominio
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475987"
---
# <a name="adding-a-sub-domain"></a>Agregar un subdominio

Los subdominios se pueden agregar al mismo inquilino o a un inquilino diferente del dominio primario. En cualquier caso, debe administrar su propia configuración dns en el sitio web del registrador. Si ha dejado que Microsoft administre la configuración dns con registros NS o si compró el dominio a Microsoft, no puede agregar subdominios sin cambiarlo primero.

Agregue primero el dominio primario y, a continuación, agregue el subdominio. Si el subdominio está en el mismo inquilino, no se necesita ninguna comprobación adicional. Si agrega el subdominio a un inquilino independiente, el registro txt DNS es necesario para la comprobación de la propiedad antes de agregar el dominio y los registros DNS adicionales para los servicios seleccionados.

- Para agregar un dominio o subdominio, siga el Asistente para agregar dominio [o](https://admin.microsoft.com/Adminportal#/Domains/Wizard)agregue el dominio o subdominio manualmente yendo a **Establecer** dominios  >    >  **Agregar dominio**.

Si es necesario:

- Para cambiar quién administra la configuración dns de un dominio existente, vaya **a Configuración** Domains , active la casilla situada junto al dominio y, a continuación, seleccione  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)Administrar **DNS**. En el asistente, seleccione **Agregar sus propios registros DNS** y complete el asistente.
- Para agregar subdominios a un dominio comprado por Microsoft, primero transfiera el dominio a otro registrador y, a continuación, realice el cambio anterior para administrar sus propios registros DNS. Para obtener instrucciones, [vea Transferir un dominio de Microsoft a otro host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Si recibe un error de que el dominio ya está en uso por otros miembros o personas de la organización, primero tendrá que asumir esta cuenta no administrada antes de usar el dominio. Para obtener instrucciones, [vea Take over an unmanaged directory as administrator in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
