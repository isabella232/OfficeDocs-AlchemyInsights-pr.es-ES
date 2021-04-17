---
title: No se puede establecer ni ver la directiva AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826108"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>No se puede establecer ni ver la directiva AllowSelfServicePurchase

Al intentar establecer o ver la directiva AllowSelfServicePurchase, recibe el siguiente mensaje de error:

*HandleError: no se pudo recuperar la directiva de producto con PolicyId 'AllowSelfServicePurchase', ErrorMessage: se cerró la conexión subyacente: se produjo un error inesperado en un envío.*

Esto puede deberse a una versión anterior de Seguridad de la capa de transporte (TLS). Para conectar el servicio MSCommerce, debe usar TLS 1.2 o posterior.  

Pruebe los pasos siguientes para habilitar o establecer el protocolo TLS en 1.2, comprobar y reintentar.
 1. En el símbolo del sistema de PowerShell (PS C: escriba el siguiente comando para establecer el protocolo \) TLS en la versión 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Compruebe los protocolos TLS en uso con el siguiente comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Reintente los comandos Get o Update según sea necesario.

