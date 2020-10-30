---
title: Solución de problemas de Microsoft defender para Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801463"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="ab2cb-102">Solución de problemas de Microsoft defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="ab2cb-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="ab2cb-103">¿Observa retrasos en la entrega de mensajes?</span><span class="sxs-lookup"><span data-stu-id="ab2cb-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="ab2cb-104">Use la opción de [entrega dinámica](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) en la Directiva de datos adjuntos seguros de ATP.</span><span class="sxs-lookup"><span data-stu-id="ab2cb-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="ab2cb-105">Esto ayudará a evitar los retrasos en los mensajes al proteger a los destinatarios de archivos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="ab2cb-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="ab2cb-106">¿Desea informar de falsos positivos o falsos negativos a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="ab2cb-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="ab2cb-107">Use este [vínculo](https://www.microsoft.com/wdsi/filesubmission/) para enviar archivos para su análisis.</span><span class="sxs-lookup"><span data-stu-id="ab2cb-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="ab2cb-108">¿Sabía que puede habilitar la protección de vínculos seguros para el correo electrónico interno que se envía entre los destinatarios de la organización?</span><span class="sxs-lookup"><span data-stu-id="ab2cb-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="ab2cb-109">Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="ab2cb-109">Follow these steps:</span></span>

  1. <span data-ttu-id="ab2cb-110">Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.</span><span class="sxs-lookup"><span data-stu-id="ab2cb-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="ab2cb-111">En el panel de navegación izquierdo, en **Administración de amenazas** , elija **Policy** \> **vínculos seguros** de directiva.</span><span class="sxs-lookup"><span data-stu-id="ab2cb-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="ab2cb-112">En la sección **directivas que se aplican a toda la organización** , seleccione la Directiva y haga clic en **Editar** .</span><span class="sxs-lookup"><span data-stu-id="ab2cb-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="ab2cb-113">En **configuración** , habilite **aplicar vínculos seguros a los mensajes enviados dentro de la organización** .</span><span class="sxs-lookup"><span data-stu-id="ab2cb-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
