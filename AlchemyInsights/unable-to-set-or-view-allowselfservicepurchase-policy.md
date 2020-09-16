---
title: No se puede establecer ni ver la Directiva de AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735216"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>No se puede establecer ni ver la Directiva de AllowSelfServicePurchase

Al intentar establecer o ver la Directiva AllowSelfServicePurchase, recibe el siguiente mensaje de error:

*HandleError: no se pudo recuperar la Directiva de producto con PolicyId ' AllowSelfServicePurchase ', ErrorMessage-se ha cerrado la conexión subyacente: se ha producido un error inesperado en un envío.*

Esto puede deberse a una versión anterior de la seguridad de la capa de transporte (TLS). Para conectar el servicio MSCommerce, debe usar TLS 1,2 o posterior.  

Pruebe los pasos siguientes para habilitar o configurar el protocolo TLS en 1,2, comprobar y reintentar.
 1. En el símbolo del sistema de PowerShell (PS C:, \) Escriba el siguiente comando para establecer el protocolo TLS en la versión 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Compruebe el protocolo o los protocolos TLS en uso, con el siguiente comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Vuelva a intentar los comandos GET o Update según sea necesario.

