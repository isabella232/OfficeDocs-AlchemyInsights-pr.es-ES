---
title: Cambiar NameServers
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 3f39bfc585e8b805424cb7ccac76f81e1b2bfda9dcd1367361fec6a668c545bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017797"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Actualizar los servidores de nombre de dominio para que señalen a Microsoft

Nota: Los cambios de Nameserver a veces pueden tardar hasta 48 horas en propagarse.
  
Para configurar su dominio en Microsoft 365, los servidores DNS en su registrador deben actualizarse. Cree o edite los registros del servidor DNS en el registrador de dominios.
  
1. Vaya al sitio web del registrador de dominios y busque el área donde puede modificar los servidores DNS.
  
2. Cree edite dos registros de servidores DNS para que coincidan con estos valores:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Guarde los cambios.

También encontrará instrucciones detalladas en este artículo: [Cambiar los servidores DNS con cualquier registrador de dominio](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  