---
title: Solución de problemas de Microsoft Defender para Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545285"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="8223f-102">Solución de problemas de Microsoft Defender para Office 365</span><span class="sxs-lookup"><span data-stu-id="8223f-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="8223f-103">**¿Nota retrasos en la entrega de mensajes?**</span><span class="sxs-lookup"><span data-stu-id="8223f-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="8223f-104">Usa la [opción Entrega dinámica](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) en tu Microsoft Defender para la directiva Office 365 Caja fuerte datos adjuntos.</span><span class="sxs-lookup"><span data-stu-id="8223f-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="8223f-105">Esto ayudará a evitar retrasos en los mensajes mientras protege a los destinatarios de archivos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="8223f-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="8223f-106">**¿Desea notificar falsos positivos o falsos negativos a Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="8223f-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="8223f-107">Use [el Explorador de envíos](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="8223f-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="8223f-108">-\*\* ¿Sabía que puede habilitar la protección de vínculos Caja fuerte para el correo electrónico interno enviado entre destinatarios dentro de su organización?\*\* Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="8223f-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="8223f-109">Vaya a [https://protection.office.com](https://protection.office.com) e inicie sesión con una cuenta de administrador global o de administrador de seguridad.</span><span class="sxs-lookup"><span data-stu-id="8223f-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="8223f-110">En el panel de navegación izquierdo en **Administración de amenazas,** elija **Directiva** \> **Caja fuerte vínculos**.</span><span class="sxs-lookup"><span data-stu-id="8223f-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="8223f-111">En la **sección Directivas que se aplican a toda la organización,** seleccione la directiva y haga clic en **Editar**.</span><span class="sxs-lookup"><span data-stu-id="8223f-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="8223f-112">En **Configuración**, habilite **Aplicar vínculos seguros a los mensajes enviados dentro de la organización**.</span><span class="sxs-lookup"><span data-stu-id="8223f-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
