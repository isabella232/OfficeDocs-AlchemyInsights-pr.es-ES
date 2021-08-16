---
title: 1065 Desuso de intervalos de direcciones IP salientes de EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031279"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Desuso de intervalos de direcciones IP salientes de EOP

Hemos detectado un posible problema con su organización que (si no se corrige antes del 26 de octubre de 2018) podría interrumpir el flujo de correo a los destinos locales o externos. Como se ha comunicado anteriormente, para simplificar la administración del intervalo de direcciones IP, estamos consolidando los intervalos de direcciones IP de Exchange Online Protection (EOP) que se usan para enviar y recibir correo electrónico fuera de Microsoft 365. Nuestro análisis indica que uno o varios de los orígenes o destinos de correo electrónico externos configurados en conectores de flujo de correo no aceptan conexiones de los intervalos de direcciones IP que se muestran [aquí](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Actúe antes del 26 de octubre para garantizar que estos orígenes y destinos acepten conexiones desde y hacia todas las [direcciones IP de EOP publicadas.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Para obtener más información acerca de este cambio, vea Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Nota:** Si anteriormente usó la publicación de DIRECCIONES IP o URL a través de HTML, XML y RSS para las actualizaciones de puntos de conexión, también debe migrar a los nuevos servicios web para automatizar estos tipos de actualizaciones. Para obtener más información, vea Microsoft 365 categorías de extremo [y Microsoft 365 dirección IP y servicio web url](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
