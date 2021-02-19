---
title: ¿Sus usuarios recibieron correo electrónico malicioso?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291809"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="7a6ca-102">¿Sus usuarios recibieron correo electrónico malicioso?</span><span class="sxs-lookup"><span data-stu-id="7a6ca-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="7a6ca-103">Ahora puede notificar el correo electrónico malintencionado a Microsoft de manera sencilla con los [envíos de administración en el Centro de seguridad y cumplimiento](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="7a6ca-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="7a6ca-104">Se escanean los mensajes que se envían [envíos de administradores](https://sip.protection.office.com/reportsubmission) y en el control flotante **detalles** se muestran los siguientes resultados:</span><span class="sxs-lookup"><span data-stu-id="7a6ca-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="7a6ca-105">Si hubo un error en la autenticación de correo electrónico del remitente en el momento de la entrega.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="7a6ca-106">Información sobre los aciertos de directiva que puedan haber afectado o invalidado el veredicto de un mensaje.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="7a6ca-107">Actualice los resultados de cancelación para ver si las direcciones URL o los archivos contenidos en el mensaje son malintencionados o no.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="7a6ca-108">Comentarios de los calificaciones</span><span class="sxs-lookup"><span data-stu-id="7a6ca-108">Feedback from graders</span></span>

<span data-ttu-id="7a6ca-109">Si se encontró una invalidación, se volverá a ejecutar una detección que se completará en unos minutos.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="7a6ca-110">Si no había un problema en la autenticación de correo electrónico o si la entrega no se vio afectada por una anulación, los comentarios de los calificadores podrían tardar hasta un día.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="7a6ca-111">Si no está de acuerdo con el veredicto final de un mensaje, dirección URL o archivo (bloqueado frente a no bloqueado), vuelva a enviar el mensaje después de un día para volver a examinarlo.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="7a6ca-112">Las probabilidades de que el veredicto cambie después de volver a enviar el mensaje son elevadas.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="7a6ca-113">Mientras tanto, puede quitar el correo electrónico malintencionado de las bandejas de entrada de los usuarios si sigue las instrucciones de [este artículo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="7a6ca-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="7a6ca-114">Los clientes con Microsoft Defender para Office 365 pueden:</span><span class="sxs-lookup"><span data-stu-id="7a6ca-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="7a6ca-115">usar [Explorador de amenazas para buscar y eliminar correo electrónico sospechoso](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="7a6ca-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="7a6ca-116">[usar vínculos seguros para bloquear el acceso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a una URL malintencionada</span><span class="sxs-lookup"><span data-stu-id="7a6ca-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="7a6ca-117">realizar un seguimiento de los usuarios que hicieron clic y accedieron a direcciones URL malintencionadas: [Ver URL de suplantación de identidad (phishing) y hacer clic en los datos de veredicto ](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="7a6ca-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="7a6ca-118">[Iniciar una investigación automatizada](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) de forma manual</span><span class="sxs-lookup"><span data-stu-id="7a6ca-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="7a6ca-119">También puede protegerse contra archivos y direcciones URL maliciosos con las siguientes instrucciones en [Protección contra archivos y direcciones URL maliciosos](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="7a6ca-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>