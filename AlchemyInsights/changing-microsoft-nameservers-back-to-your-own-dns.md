---
title: Cambiar los servidores de nombres de Microsoft para volver a administrar sus propios registros DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481893"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Cambiar los servidores de nombres de Microsoft para volver a administrar sus propios registros DNS

Anteriormente ha cambiado los registros NS para que apunten a Microsoft (ns1.bdm.microsoftonline.com), pero ahora ha decidido administrar sus propios registros DNS:

En el sitio web del registrador de dominios, vuelva a cambiar el servidor de nombres a su registrador o a la configuración anterior. Si no está familiarizado con DNS, póngase en contacto con el soporte técnico en el registrador de dominios. Tenga en cuenta que los cambios del servidor de nombres pueden tardar hasta 48 horas en propagarse. 

1. En el portal de administración de Microsoft 365, vaya a **Configuración** > [**Dominios**](https://admin.microsoft.com/Adminportal/Home#/Domains), seleccione la casilla junto al dominio y seleccione **Administrar DNS**. 

2. En el asistente, seleccione **Agregar sus propios registros DNS** y complete el asistente. Esto cambia la forma en que se administra el DNS y, a continuación, permite agregar los registros DNS personalizados necesarios para admitir los servicios seleccionados.

Como alternativa, si ha cambiado sus registros de servidor de nombres a Microsoft y tiene un sitio web, puede añadir registros DNS para el sitio web en lugar de volver a cambiar los servidores de nombres. Para obtener más información, consulte [Actualizar los registros DNS para mantener su sitio web con su proveedor de hospedaje actual](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


