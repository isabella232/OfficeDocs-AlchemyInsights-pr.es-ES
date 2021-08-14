---
title: Solucionar problemas de acceso denegado
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957990"
---
# <a name="troubleshoot-access-denied-messages"></a>Solucionar problemas de acceso denegado

Si recibe un mensaje de acceso denegado al intentar examinar un sitio de Sharepoint Online, consulte los artículos siguientes.

**Agregar y licenciar al usuario**

Asegúrese de asignar [licencias a usuarios de Microsoft 365 para empresas](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Asignar permisos**

Si al usuario se le ha asignado una licencia de Sharepoint y sigue recibiendo un mensaje de acceso denegado, asegúrese de que tiene asignado el [nivel de permiso adecuado](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Considere la posibilidad de usar la característica de solicitud de acceso**

La [característica de solicitud de](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) acceso permite a los usuarios solicitar acceso al contenido que actualmente no tienen permiso para ver. 

**Permitir script personalizado puede causar problemas de acceso denegado**

Hay ciertos escenarios en los que la característica "Permitir script personalizado" puede estar presentando un acceso denegado. Para obtener una lista de características afectadas, consideraciones de seguridad y la capacidad de deshabilitar la característica. Visite , [Permitir o impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Nota: Si un sitio OneDrive o SharePoint no está disponible para varios usuarios que tenían acceso anteriormente, puede haber un problema de servicio temporal. [Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).


  

