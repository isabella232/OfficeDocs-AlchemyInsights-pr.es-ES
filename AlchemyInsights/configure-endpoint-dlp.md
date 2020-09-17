---
title: Configurar DLP en punto de conexión
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812132"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="51df7-102">Configurar DLP en punto de conexión</span><span class="sxs-lookup"><span data-stu-id="51df7-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="51df7-103">DLP en punto de conexión de Microsoft le permite ampliar la funcionalidad de protección y supervisión de DLP a información confidencial en dispositivos con Windows 10.</span><span class="sxs-lookup"><span data-stu-id="51df7-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="51df7-104">Después de que los dispositivos estén integrados en la administración de dispositivos, puede crear directivas DLP para aplicar acciones de protección en los elementos.</span><span class="sxs-lookup"><span data-stu-id="51df7-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="51df7-105">El explorador de actividades se puede usar para supervisar la actividad de elementos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="51df7-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="51df7-106">Para más información, consulte [Incorporación de dispositivos en la administración de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="51df7-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="51df7-107">Para empezar a usar DLP en punto de conexión:</span><span class="sxs-lookup"><span data-stu-id="51df7-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="51df7-108">Asegúrese de que tiene la licencia de SKU o suscripciones adecuadas.</span><span class="sxs-lookup"><span data-stu-id="51df7-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="51df7-109">Para más información, consulte [Licencia de SKU o suscripciones](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="51df7-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="51df7-110">Compruebe los permisos necesarios para habilitar la administración de dispositivos, acceder a la página de incorporación o activar o desactivar la supervisión de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="51df7-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="51df7-111">Para más información, consulte [Permisos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="51df7-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="51df7-112">Incorpore dispositivos en la administración de dispositivos siguiendo el procedimiento de incorporación de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="51df7-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="51df7-113">Si no encuentra la opción de Incorporación de dispositivos (vista previa) en la **Configuración** de cumplimiento de M365, confirme que tiene la licencia y los permisos adecuados que se mencionan anteriormente.</span><span class="sxs-lookup"><span data-stu-id="51df7-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="51df7-114">Para más información, consulte [Incorporación de dispositivos](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="51df7-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="51df7-115">Cree directivas DLP para proteger sus elementos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="51df7-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="51df7-116">Para más información, consulte [Escenarios de directiva DLP de los puntos de conexión](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="51df7-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="51df7-117">Para más información sobre DLP en punto de conexión de Microsoft, consulte [Obtener información sobre la prevención de pérdida de datos en punto de conexión de Microsoft 365 (vista previa)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="51df7-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>