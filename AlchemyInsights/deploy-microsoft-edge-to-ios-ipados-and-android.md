---
title: Implementar Microsoft Edge en iOS, iPadOS y Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178015"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="65567-102">Implementar Microsoft Edge en iOS, iPadOS y Android</span><span class="sxs-lookup"><span data-stu-id="65567-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="65567-103">El escenario guiado que se resume a continuación le ayudará a asignar Microsoft Edge a los usuarios de dispositivos iOS, iPadOS y Android.</span><span class="sxs-lookup"><span data-stu-id="65567-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="65567-104">Si bloqueó a los usuarios para que no puedan inscribirse en dispositivos móviles, este escenario guiado no funcionará y los usuarios necesitarán instalar Microsoft Edge por su cuenta.</span><span class="sxs-lookup"><span data-stu-id="65567-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="65567-105">El escenario guiado incluye los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="65567-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="65567-106">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="65567-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="65567-107">Introducción</span><span class="sxs-lookup"><span data-stu-id="65567-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="65567-108">Conceptos básicos</span><span class="sxs-lookup"><span data-stu-id="65567-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="65567-109">Configuración</span><span class="sxs-lookup"><span data-stu-id="65567-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="65567-110">Asignaciones</span><span class="sxs-lookup"><span data-stu-id="65567-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="65567-111">Revisión y creación</span><span class="sxs-lookup"><span data-stu-id="65567-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="65567-112">Después de completar los pasos del escenario guiado, las directivas de Microsoft Intune habilitarán las características siguientes de Microsoft Edge para empresas:</span><span class="sxs-lookup"><span data-stu-id="65567-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="65567-113">Identidad doble</span><span class="sxs-lookup"><span data-stu-id="65567-113">Dual identity</span></span>
- <span data-ttu-id="65567-114">Integración con la directiva de protección de aplicaciones de Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="65567-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="65567-115">Integración con Azure Active Directory Application Proxy</span><span class="sxs-lookup"><span data-stu-id="65567-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="65567-116">Favoritos administrados y accesos directos a la página principal</span><span class="sxs-lookup"><span data-stu-id="65567-116">Managed favorites and home page shortcuts</span></span>
