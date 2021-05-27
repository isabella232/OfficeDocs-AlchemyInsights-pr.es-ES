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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657946"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="78811-102">Configurar DLP en punto de conexión</span><span class="sxs-lookup"><span data-stu-id="78811-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="78811-103">DLP en punto de conexión de Microsoft le permite ampliar la funcionalidad de protección y supervisión de DLP a información confidencial en dispositivos con Windows 10.</span><span class="sxs-lookup"><span data-stu-id="78811-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="78811-104">Después de que los dispositivos estén integrados en la administración de dispositivos, puede crear directivas DLP para aplicar acciones de protección en los elementos.</span><span class="sxs-lookup"><span data-stu-id="78811-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="78811-105">El explorador de actividades se puede usar para supervisar la actividad de elementos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="78811-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="78811-106">Para más información, consulte [Incorporación de dispositivos en la administración de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="78811-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="78811-107">Para empezar a usar DLP en punto de conexión:</span><span class="sxs-lookup"><span data-stu-id="78811-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="78811-108">Asegúrese de que tiene la licencia de SKU o suscripciones adecuadas.</span><span class="sxs-lookup"><span data-stu-id="78811-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="78811-109">Para más información, consulte [Licencia de SKU o suscripciones](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="78811-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="78811-p103">Compruebe los permisos necesarios para habilitar la administración de dispositivos, acceder a la página de incorporación o activar o desactivar la supervisión de dispositivos. Para más información, consulte [Permisos](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="78811-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="78811-112">Incorpore dispositivos en la Administración de dispositivos siguiendo el procedimiento de incorporación de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="78811-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="78811-113">Para más información, consulte [Incorporación de dispositivos](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="78811-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="78811-114">Cree directivas DLP para proteger sus elementos confidenciales.</span><span class="sxs-lookup"><span data-stu-id="78811-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="78811-115">Para más información, consulte [Escenarios de directiva DLP de los puntos de conexión](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="78811-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="78811-116">Para más información sobre DLP en punto de conexión de Microsoft, consulte [Obtener información sobre la prevención de pérdida de datos en punto de conexión de Microsoft 365 (vista previa)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="78811-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="78811-117">**Pasos importantes de recopilación de datos, si se necesita Soporte técnico:**</span><span class="sxs-lookup"><span data-stu-id="78811-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="78811-118">Descargue la [Versión preliminar de MDATP Client Analyzer](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="78811-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="78811-119">Ejecute la herramienta como administrador en la ventana de símbolo del sistema:</span><span class="sxs-lookup"><span data-stu-id="78811-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="78811-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="78811-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="78811-121">Cuando aparezca el mensaje **Escriba el número de minutos para recopilar seguimientos:**, escriba el número de minutos necesarios para ejecutar el escenario</span><span class="sxs-lookup"><span data-stu-id="78811-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="78811-122">Ejecute el escenario.</span><span class="sxs-lookup"><span data-stu-id="78811-122">Run the scenario.</span></span>

<span data-ttu-id="78811-123">Recopile el archivo zip resultante para entregarlo al agente de soporte.</span><span class="sxs-lookup"><span data-stu-id="78811-123">Collect the Zip file output to give to the Support agent.</span></span>
