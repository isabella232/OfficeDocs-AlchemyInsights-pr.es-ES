---
title: Usar Microsoft Intune para administrar el acceso web en Microsoft Edge para iOS y Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617341"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1520f-102">Usar Microsoft Intune para administrar el acceso web en Microsoft Edge para iOS y Android</span><span class="sxs-lookup"><span data-stu-id="1520f-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1520f-103">Microsoft Edge para iOS y Android permite a un usuario explorar la web desde varios perfiles completamente separados.</span><span class="sxs-lookup"><span data-stu-id="1520f-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1520f-104">Las capacidades de protección más amplias de los datos de Microsoft 365 se encuentran disponibles al suscribirse a Enterprise Mobility + Security Suite, que incluye las características de Microsoft Intune y Azure Active Directory Premium, como el acceso condicional.</span><span class="sxs-lookup"><span data-stu-id="1520f-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1520f-105">Como mínimo, querrá implementar una directiva de acceso condicional que (1) permita a los usuarios conectarse desde dispositivos móviles a Microsoft Edge para iOS y Android, y que (2) implemente una directiva de protección de aplicaciones de Microsoft Intune que ofrezca una experiencia de exploración protegida.</span><span class="sxs-lookup"><span data-stu-id="1520f-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1520f-106">Para comprender cómo se pueden usar las directivas y el acceso condicional, vea:</span><span class="sxs-lookup"><span data-stu-id="1520f-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1520f-107">Aplicar directivas de acceso condicional de Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1520f-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1520f-108">Crear directivas de protección de aplicaciones de Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1520f-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1520f-109">Usar el inicio de sesión único para aplicaciones web conectadas con Azure Active Directory en exploradores protegidos por directiva</span><span class="sxs-lookup"><span data-stu-id="1520f-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1520f-110">Usar la configuración de la aplicación para administrar la experiencia de navegación</span><span class="sxs-lookup"><span data-stu-id="1520f-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1520f-111">Permitir el uso de solo cuentas de trabajo y centro educativo</span><span class="sxs-lookup"><span data-stu-id="1520f-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1520f-112">Implementación de directivas de configuración generales de la aplicación</span><span class="sxs-lookup"><span data-stu-id="1520f-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1520f-113">Implementación de directivas de configuración de aplicaciones para la protección de datos</span><span class="sxs-lookup"><span data-stu-id="1520f-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1520f-114">Usar Microsoft Endpoint Manager para implementar directivas de configuración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="1520f-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1520f-115">Para obtener información sobre cómo acceder a los registros de aplicaciones administradas, vea [usar Microsoft Edge para iOS y Android para acceder a los registros de aplicaciones administradas](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="1520f-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
