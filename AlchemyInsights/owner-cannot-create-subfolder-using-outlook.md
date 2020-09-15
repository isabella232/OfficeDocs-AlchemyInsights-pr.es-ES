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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="5f313-102">El propietario no puede crear una subcarpeta con Outlook</span><span class="sxs-lookup"><span data-stu-id="5f313-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="5f313-103">**Hay un problema en curso con los propietarios de las carpetas públicas al crear subcarpetas con Outlook. El problema se corregirá pronto.**</span><span class="sxs-lookup"><span data-stu-id="5f313-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="5f313-104">Mientras tanto, pruebe una de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="5f313-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="5f313-105">Usar Outlook para MAC para crear la subcarpeta, puesto que el problema afecta solo a Outlook para ventanas de escritorio (todas las versiones)</span><span class="sxs-lookup"><span data-stu-id="5f313-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="5f313-106">Pedir al administrador que cree la subcarpeta con el Shell de EXO o con EAC</span><span class="sxs-lookup"><span data-stu-id="5f313-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="5f313-107">Cambiar DefaultPublicFolderMailbox/EffectivePublicFolderMailbox del usuario a otro buzón que no sea el buzón de contenido de la carpeta causante del problema</span><span class="sxs-lookup"><span data-stu-id="5f313-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="5f313-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="5f313-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="5f313-109">Esperar una hora y reiniciar el cliente de Outlook</span><span class="sxs-lookup"><span data-stu-id="5f313-109">Wait for an hour, restart outlook client</span></span>