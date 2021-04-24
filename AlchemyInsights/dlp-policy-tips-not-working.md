---
title: Sugerencias de directivas dlp no funcionan
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958719"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="b5781-102">Problemas de sugerencias de directiva DLP</span><span class="sxs-lookup"><span data-stu-id="b5781-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="b5781-103">**Importante**: durante estos tiempos, se siguen pasos para asegurarse de que los servicios de SharePoint Online y OneDrive estén altamente disponibles. Para obtener más información, visite [Ajustes temporales de características de SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b5781-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b5781-104">Para configurar las sugerencias de directiva en la directiva DLP en el Centro de seguridad & cumplimiento en modo de aplicación completa, haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="b5781-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="b5781-105">Asegúrese de que las sugerencias de **directiva se hayan habilitado** en la regla DLP.</span><span class="sxs-lookup"><span data-stu-id="b5781-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="b5781-106">Para ver los pasos, vea [Enviar notificaciones por correo electrónico y mostrar sugerencias de directivas para directivas DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="b5781-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="b5781-107">Asegúrese de que el contenido coincide con lo necesario para desencadenar la regla descrita en [Definiciones de](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)entidad de tipo de información confidencial .</span><span class="sxs-lookup"><span data-stu-id="b5781-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="b5781-108">Las sugerencias de directiva se muestran en OWA y Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5781-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="b5781-109">Sin embargo, al usar Outlook 2013 o versiones posteriores, las sugerencias de directiva solo se muestran en determinadas condiciones.</span><span class="sxs-lookup"><span data-stu-id="b5781-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="b5781-110">Para obtener la lista de condiciones específicas, vea [Condiciones admitidas para Outlook 2013](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)o posterior para mostrar sugerencias de directiva .</span><span class="sxs-lookup"><span data-stu-id="b5781-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="b5781-111">Para obtener información sobre las sugerencias de directiva DLP, vea [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and Support Matrix for DLP Policy [Tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span><span class="sxs-lookup"><span data-stu-id="b5781-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>