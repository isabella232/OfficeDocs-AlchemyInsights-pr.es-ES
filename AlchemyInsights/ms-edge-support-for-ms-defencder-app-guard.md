---
title: Soporte de Microsoft Edge para la protección de aplicaciones de Microsoft defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576635"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="49dd8-102">Soporte de Microsoft Edge para la protección de aplicaciones de Microsoft defender</span><span class="sxs-lookup"><span data-stu-id="49dd8-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="49dd8-103">Diseñada para Windows 10 y Microsoft Edge, la protección de aplicaciones usa un enfoque de aislamiento de hardware que permite a un usuario navegar por un sitio que no es de confianza desde dentro de un contenedor aislado, compatible con Hyper-V, separado del sistema operativo host.</span><span class="sxs-lookup"><span data-stu-id="49dd8-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="49dd8-104">Un administrador de la empresa define una lista de sitios web de confianza, recursos de la nube y redes internas.</span><span class="sxs-lookup"><span data-stu-id="49dd8-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="49dd8-105">Cuando un usuario visita un sitio que no se encuentra en la lista, Microsoft Edge abrirá el sitio en el contenedor.</span><span class="sxs-lookup"><span data-stu-id="49dd8-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="49dd8-106">Esto significa que si el sitio resulta ser malintencionado, el equipo host seguirá protegido y el atacante no recibirá los datos de la empresa.</span><span class="sxs-lookup"><span data-stu-id="49dd8-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="49dd8-107">La instalación de extensiones en el contenedor es compatible con la versión 81 de Microsoft Edge y puede controlarse a través de una directiva.</span><span class="sxs-lookup"><span data-stu-id="49dd8-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="49dd8-108">La dirección updateURL que se usa en la Directiva ExtensionInstallForcelist debe agregarse como un recurso neutro en las directivas de aislamiento de red que usa la protección de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="49dd8-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="49dd8-109">Para obtener más información, vea [compatibilidad de Microsoft Edge con protección de aplicaciones de Microsoft defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="49dd8-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
