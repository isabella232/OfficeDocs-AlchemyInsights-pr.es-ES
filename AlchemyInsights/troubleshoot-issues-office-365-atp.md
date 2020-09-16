---
title: Solución de problemas con la protección contra amenazas avanzada de Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758082"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="d5be0-102">Solucionar problemas con Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="d5be0-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="d5be0-103">¿Hay **retrasos en la entrega de mensajes de correo electrónico**?</span><span class="sxs-lookup"><span data-stu-id="d5be0-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="d5be0-104">Pruebe a usar la opción de entrega dinámica para las directivas de datos adjuntos seguros de ATP.</span><span class="sxs-lookup"><span data-stu-id="d5be0-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="d5be0-105">Esto evitará los retrasos en la entrega de mensajes de correo electrónico al proteger a los destinatarios de archivos malintencionados.</span><span class="sxs-lookup"><span data-stu-id="d5be0-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="d5be0-106">**¿Desea informar de falsos positivos o falsos negativos**?</span><span class="sxs-lookup"><span data-stu-id="d5be0-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="d5be0-107">Use este vínculo para enviar el archivo para su análisis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="d5be0-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="d5be0-108">**¿Sabía que puede habilitar la protección de vínculos seguros de ATP para el correo electrónico que se envía entre las personas de su organización**?</span><span class="sxs-lookup"><span data-stu-id="d5be0-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="d5be0-109">Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="d5be0-109">Follow these steps:</span></span>
    1. <span data-ttu-id="d5be0-110">Vaya a https://protection.office.com e inicie sesión.</span><span class="sxs-lookup"><span data-stu-id="d5be0-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="d5be0-111">Vaya a **Threat management**  >  **Policy**  >  **vínculos seguros**de la Directiva de administración de amenazas.</span><span class="sxs-lookup"><span data-stu-id="d5be0-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="d5be0-112">En **directivas que se aplican a destinatarios específicos**, edite (o agregue) una directiva.</span><span class="sxs-lookup"><span data-stu-id="d5be0-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="d5be0-113">Seleccione **aplicar vínculos seguros a los mensajes enviados dentro de la organización**.</span><span class="sxs-lookup"><span data-stu-id="d5be0-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="d5be0-114">Guarde la Directiva y espere unos 30 minutos para que los cambios funcionen en el centro de proceso de información.</span><span class="sxs-lookup"><span data-stu-id="d5be0-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="d5be0-115">Para obtener más ayuda con ATP, consulte [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="d5be0-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>