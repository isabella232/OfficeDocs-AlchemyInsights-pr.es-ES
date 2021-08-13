---
title: Restringir SharePoint Online al modo clásico
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958818"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir SharePoint Online al modo clásico

Algunas organizaciones aún requieren la experiencia del modo clásico. Aunque no hay planes para quitar el modo clásico en un nivel granular, ya no es posible restringir toda una organización (inquilino) al modo clásico para listas y bibliotecas.

El administrador tendrá las siguientes opciones para administrar listas y bibliotecas individuales en modo clásico mediante modificadores de exclusión pormenorizados que proporcionamos en los siguientes niveles:

- colección de sitios
- sitio
- lista
- biblioteca

Además, las listas que usan determinadas características y personalizaciones que no son compatibles con modern seguirán cambiando automáticamente al modo clásico.

A partir del 1 de abril de 2019, el proceso para deshabilitar el nivel de inquilino optar por no participar en listas modernas y bibliotecas se iniciará y continuará hasta el 31 de mayo de 2019.  Las listas y bibliotecas que están en modo clásico como resultado de la exclusión del inquilino se cambiarán automáticamente a modernas.

Si necesita el modo clásico, vea más información [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) aquí y instrucciones de Powershell pnP aquí que describen las opciones y las herramientas que puede usar hoy para usar la experiencia del modo clásico. [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)
