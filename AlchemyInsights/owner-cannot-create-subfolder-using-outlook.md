---
title: El propietario no puede crear una subcarpeta con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716653"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="4939c-102">El propietario no puede crear una subcarpeta con Outlook</span><span class="sxs-lookup"><span data-stu-id="4939c-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="4939c-103">**Hay un problema en curso con los propietarios de las carpetas públicas al crear subcarpetas con Outlook. El problema se corregirá prónto.**</span><span class="sxs-lookup"><span data-stu-id="4939c-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="4939c-104">Mientras tanto, pruebe una de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="4939c-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="4939c-105">Usar Outlook para MAC para crear la subcarpeta, puesto que el problema afecta solo a Outlook para ventanas de escritorio (todas las versiones)</span><span class="sxs-lookup"><span data-stu-id="4939c-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="4939c-106">Pedir al administrador que cree la subcarpeta con el Shell de EXO o con EAC</span><span class="sxs-lookup"><span data-stu-id="4939c-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="4939c-107">Cambiar DefaultPublicFolderMailbox/EffectivePublicFolderMailbox del usuario a otro buzón que no sea el buzón de contenido de la carpeta causante del problema</span><span class="sxs-lookup"><span data-stu-id="4939c-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="4939c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="4939c-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="4939c-109">Esperar una hora y reiniciar el cliente de outlook</span><span class="sxs-lookup"><span data-stu-id="4939c-109">Wait for an hour, restart outlook client</span></span>