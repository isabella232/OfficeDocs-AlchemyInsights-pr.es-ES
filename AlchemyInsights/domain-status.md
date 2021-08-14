---
title: 'Estado del dominio: sin servicios seleccionados'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1ddf6475e7cf466a39f76486e0f809097917657bc8f4ae7f7f2b516657308f39
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947460"
---
# <a name="domain-status---no-services-selected"></a>Estado del dominio: sin servicios seleccionados

**Ningún servicio** seleccionado significa que no ha seleccionado ningún servicio de Microsoft 365, como Exchange Online, Skype Empresarial o Intune, ni Administración de dispositivos móviles para Microsoft 365 que usar con su dominio personalizado. Si usa Exchange híbrido (Exchange local con Exchange Online) o filtrado de correo no deseado externo con Exchange y ningún otro servicios Microsoft, puede omitir este mensaje. El estado del dominio solo está disponible para dominios conectados directamente al servicio.

Para seleccionar servicios para su dominio:

1. Desde **Configuración**, active la casilla situada junto al dominio con el mensaje de estado No hay servicios  >  [](https://admin.microsoft.com/Adminportal/Home) **seleccionados**.
1. Seleccione **Administrar DNS** para iniciar el Asistente para la instalación de dominios.
    - Si elige **Agregar sus propios registros DNS,** asegúrese de seleccionar un servicio cuando se le pida. Puede haber más servicios disponibles en **Opciones avanzadas**.
    - Si elige Permitir **que Microsoft agregue sus registros DNS** o Más opciones Configurar mis servicios en línea para mí, todos los servicios disponibles se   >   sugieren y seleccionan automáticamente.
1. Continúe con el asistente para completar la configuración de DNS y las opciones de servicio.
 
Para obtener ayuda adicional para configurar el dominio, vea [Agregar registros DNS para conectar el dominio](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

