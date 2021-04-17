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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="e0a92-102">El propietario no puede crear una subcarpeta con Outlook</span><span class="sxs-lookup"><span data-stu-id="e0a92-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="e0a92-103">**Hay un problema en curso con los propietarios de las carpetas públicas al crear subcarpetas con Outlook. El problema se corregirá pronto.**</span><span class="sxs-lookup"><span data-stu-id="e0a92-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="e0a92-104">Mientras tanto, pruebe una de las siguientes soluciones:</span><span class="sxs-lookup"><span data-stu-id="e0a92-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="e0a92-105">Usar Outlook para MAC para crear la subcarpeta, puesto que el problema afecta solo a Outlook para ventanas de escritorio (todas las versiones)</span><span class="sxs-lookup"><span data-stu-id="e0a92-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="e0a92-106">Pedir al administrador que cree la subcarpeta con el Shell de EXO o con EAC</span><span class="sxs-lookup"><span data-stu-id="e0a92-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="e0a92-107">Cambiar DefaultPublicFolderMailbox/EffectivePublicFolderMailbox del usuario a otro buzón que no sea el buzón de contenido de la carpeta causante del problema</span><span class="sxs-lookup"><span data-stu-id="e0a92-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="e0a92-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="e0a92-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="e0a92-109">Esperar una hora y reiniciar el cliente de Outlook</span><span class="sxs-lookup"><span data-stu-id="e0a92-109">Wait for an hour, restart outlook client</span></span>