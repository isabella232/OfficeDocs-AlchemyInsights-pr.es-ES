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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020209"
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

