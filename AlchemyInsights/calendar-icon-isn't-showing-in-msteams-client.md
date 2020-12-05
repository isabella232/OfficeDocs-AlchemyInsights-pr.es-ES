---
title: El icono de calendario no se muestra en el cliente de Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576620"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="0b2fd-102">El icono de calendario no se muestra en el cliente de Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0b2fd-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="0b2fd-103">La ficha **calendario** en Microsoft Teams requiere acceso a un buzón de Exchange a través de los servicios web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b2fd-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="0b2fd-104">El buzón de Exchange puede estar en línea o local.</span><span class="sxs-lookup"><span data-stu-id="0b2fd-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="0b2fd-105">Para los usuarios en línea que no ven la ficha **calendario** , asegúrese [de que tienen licencia para un buzón de Exchange Online y el buzón de correo está habilitado](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0b2fd-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="0b2fd-106">Si los usuarios están hospedados en local, debe confirmar que la configuración híbrida es correcta.</span><span class="sxs-lookup"><span data-stu-id="0b2fd-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="0b2fd-107">Use el [Asistente para la configuración híbrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) para solucionar el problema.</span><span class="sxs-lookup"><span data-stu-id="0b2fd-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="0b2fd-108">Tenga en cuenta que [Teams requiere Exchange 2016 CU3 o una versión superior](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="0b2fd-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="0b2fd-109">Para obtener más información y pasos para la solución de problemas, consulte [solucionar problemas de interacción de Microsoft Teams y Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="0b2fd-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
