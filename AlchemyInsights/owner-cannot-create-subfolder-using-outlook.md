---
title: El propietario no puede crear una subcarpeta con Outlook
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
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665735"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>El propietario no puede crear una subcarpeta con Outlook

**Hay un problema en curso con los propietarios de las carpetas públicas al crear subcarpetas con Outlook. El problema se corregirá pronto.**

Mientras tanto, pruebe una de las siguientes soluciones:

1. Usar Outlook para MAC para crear la subcarpeta, puesto que el problema afecta solo a Outlook para ventanas de escritorio (todas las versiones)
2. Pedir al administrador que cree la subcarpeta con el Shell de EXO o con EAC
3. Cambiar DefaultPublicFolderMailbox/EffectivePublicFolderMailbox del usuario a otro buzón que no sea el buzón de contenido de la carpeta causante del problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Esperar una hora y reiniciar el cliente de Outlook