---
title: El propietario no puede crear una subcarpeta con Outlook
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
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836152"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>El propietario no puede crear una subcarpeta con Outlook

**Hay un problema en curso con los propietarios de las carpetas públicas al crear subcarpetas con Outlook. El problema se corregirá pronto.**

Mientras tanto, pruebe una de las siguientes soluciones:

1. Usar Outlook para MAC para crear la subcarpeta, puesto que el problema afecta solo a Outlook para ventanas de escritorio (todas las versiones)
2. Pedir al administrador que cree la subcarpeta con el Shell de EXO o con EAC
3. Cambiar DefaultPublicFolderMailbox/EffectivePublicFolderMailbox del usuario a otro buzón que no sea el buzón de contenido de la carpeta causante del problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Esperar una hora y reiniciar el cliente de Outlook