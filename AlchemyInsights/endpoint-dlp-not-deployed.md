---
title: DLP en punto de conexión no implementado en el dispositivo del usuario
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694814"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="24a15-102">DLP en punto de conexión no implementado en el dispositivo del usuario</span><span class="sxs-lookup"><span data-stu-id="24a15-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="24a15-103">Si la configuración de prevención de pérdida de datos (DLP) en punto de conexión no se ha aplicado en el dispositivo de un usuario, confirme que cumple estos requisitos:</span><span class="sxs-lookup"><span data-stu-id="24a15-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="24a15-104">La compilación 1809 o posterior de Windows 10 x64 está instalada en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="24a15-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="24a15-105">Está instalada la versión 4.18.2009.7 o una posterior del cliente antimalware.</span><span class="sxs-lookup"><span data-stu-id="24a15-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="24a15-106">El dispositivo cumple **una** de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="24a15-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="24a15-107">Unido a Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="24a15-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="24a15-108">Unido a Azure AD híbrido </span><span class="sxs-lookup"><span data-stu-id="24a15-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="24a15-109">Registrado en AAD</span><span class="sxs-lookup"><span data-stu-id="24a15-109">AAD registered</span></span>

- <span data-ttu-id="24a15-110">Para aplicar acciones de directiva, asegúrese de que el explorador Microsoft Chromium Edge está instalado en el dispositivo de punto de conexión.</span><span class="sxs-lookup"><span data-stu-id="24a15-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="24a15-111">Para ver los requisitos adicionales para implementar DLP en punto de conexión, vea [Introducción a la Prevención de pérdida de datos en punto de conexión](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="24a15-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>