---
title: 902 (Errores de sincronización debidos a objetos duplicados)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998817"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Errores de sincronización debido a objetos duplicados

Es posible que reciba uno de los siguientes mensajes de error cuando la sincronización de directorios finalice en Microsoft 365:

- No se puede actualizar este objeto en Microsoft Online Services porque los siguientes atributos asociados a este objeto tienen valores que ya pueden estar asociados con otro objeto en el directorio local.

- Ya existe un objeto sincronizado con la misma dirección proxy en el directorio Microsoft Online Services servidor.

- No se puede actualizar este objeto porque los siguientes atributos asociados a este objeto tienen valores que pueden estar asociados a otro objeto en los servicios de directorio local: UserPrincipalName.

Para identificar y corregir el problema, descargue y ejecute la herramienta de corrección de [errores IdFix DirSync](https://github.com/Microsoft/idfix).

Para obtener más información, [vea KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
