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
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326594"
---
# <a name="domain-status---no-services-selected"></a>Estado del dominio: sin servicios seleccionados

**Ningún servicio** seleccionado significa que no ha seleccionado ningún servicio de Microsoft 365, como Exchange Online, Skype Empresarial o Intune, ni Administración de dispositivos móviles para Microsoft 365 que usar con su dominio personalizado. Si usa Exchange híbrido (Exchange local con Exchange Online) o filtrado de correo no deseado externo con Exchange y ningún otro servicios Microsoft, puede omitir este mensaje. El estado del dominio solo está disponible para dominios conectados directamente al servicio.

Para seleccionar servicios para su dominio:

1. Desde **Configuración**, active la casilla situada junto al dominio con el mensaje de estado No hay servicios  >  [](https://admin.microsoft.com/Adminportal/Home) **seleccionados**.
1. Seleccione **Administrar DNS** para iniciar el Asistente para la instalación de dominios.
    - Si elige **Agregar sus propios registros DNS,** asegúrese de seleccionar un servicio cuando se le pida. Puede haber más servicios disponibles en **Opciones avanzadas**.
    - Si elige Permitir **que Microsoft agregue sus registros DNS** o Más opciones Configurar mis servicios en línea para mí, todos los servicios disponibles se   >   sugieren y seleccionan automáticamente.
1. Continúe con el asistente para completar la configuración de DNS y las opciones de servicio.
 
Para obtener ayuda adicional para configurar el dominio, vea [Agregar registros DNS para conectar el dominio](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

