---
title: 'Problemas de rendimiento: SharePoint o OneDrive'
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771261"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive son lentos, inaccesibles o no disponibles para varios usuarios

Si un sitio de OneDrive o SharePoint no está disponible para varios usuarios que anteriormente tenían acceso, es posible que haya un problema de servicio temporal. [Compruebe el panel de estado del servicio](https://portal.office.com/adminportal/home#/servicehealth).

**Agregar y conceder una licencia al usuario**

Asegúrese de [asignar licencias a los usuarios en Microsoft 365 para empresas](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Asignar permisos**

Si al usuario se le ha asignado una licencia de SharePoint y sigue recibiendo un mensaje de acceso denegado, asegúrese de que tiene asignado el [nivel de permisos adecuado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Considerar el uso de la característica de solicitud de acceso**

La [característica de solicitud de acceso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite que las personas soliciten acceso al contenido que actualmente no tiene permiso para ver.

**Permitir el script personalizado puede provocar problemas de denegación de acceso**

Hay algunos escenarios en los que la característica *permitir scripts personalizados* puede presentar un acceso denegado. Para obtener una lista de características afectadas, consideraciones de seguridad y la posibilidad de deshabilitar la característica. Visite [permitir o impedir scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

