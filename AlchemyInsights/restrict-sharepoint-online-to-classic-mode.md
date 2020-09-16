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
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751439"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restringir SharePoint Online al modo clásico

Algunas organizaciones todavía necesitan la experiencia de modo clásico. Aunque no hay planes para quitar el modo clásico en un nivel granular, ya no es posible restringir una organización completa (inquilino) al modo clásico para listas y bibliotecas.

El administrador tendrá las siguientes opciones para administrar listas y bibliotecas individuales en modo clásico mediante modificadores de exclusión granulares que proporcionamos en los siguientes niveles:

- colección de sitios
- sitio
- lista
- Biblioteca

Además, las listas que usan determinadas características y personalizaciones que no son compatibles con Modern seguirán cambiando automáticamente al modo clásico.

A partir del 1 de abril de 2019, el proceso para deshabilitar el nivel de inquilino no participar en la lista y las bibliotecas modernas se iniciará y continuará hasta el 31 de mayo de 2019.  Las listas y bibliotecas que se encuentran en modo clásico como resultado de la cancelación de inquilino se desplazarán automáticamente a moderna.

Si necesita el modo clásico, vea [aquí](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) más información [aquí](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) y instrucciones de PowerShell PNP que describe las opciones y las herramientas que puede usar hoy para usar la experiencia de modo clásico.
