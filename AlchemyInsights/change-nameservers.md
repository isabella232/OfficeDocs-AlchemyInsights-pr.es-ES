---
title: Cambiar NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714741"
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
  