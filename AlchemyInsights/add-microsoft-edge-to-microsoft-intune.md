---
title: Agregar Microsoft Edge a Microsoft Intune
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
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178014"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="c79e6-102">Agregar Microsoft Edge a Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c79e6-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="c79e6-103">Para poder implementar, configurar, supervisar y proteger Microsoft Edge para Windows 10, primero debe agregarlo a Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c79e6-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="c79e6-104">Intune es compatible con Microsoft Edge 77 y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="c79e6-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="c79e6-105">Intune detectará las instalaciones preexistentes de Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c79e6-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="c79e6-106">Si Microsoft Edge está instalado en el contexto del usuario, una instalación del sistema sobrescribirá la instalación en el contexto del usuario.</span><span class="sxs-lookup"><span data-stu-id="c79e6-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="c79e6-107">Si Microsoft Edge se instala en el contexto del sistema, se notifica que la instalación se realizó correctamente.</span><span class="sxs-lookup"><span data-stu-id="c79e6-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="c79e6-108">Microsoft Edge 77 preinstalado y versiones posteriores, para todos los canales en el contexto del usuario, se sobrescriben con Microsoft Edge instalado en el contexto del sistema.</span><span class="sxs-lookup"><span data-stu-id="c79e6-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="c79e6-109">**Requisito previo**</span><span class="sxs-lookup"><span data-stu-id="c79e6-109">**Prerequisite**</span></span>

<span data-ttu-id="c79e6-110">Windows 10, versión 1709 o posteriores.</span><span class="sxs-lookup"><span data-stu-id="c79e6-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="c79e6-111">**Pasos para agregar Edge a Intune**</span><span class="sxs-lookup"><span data-stu-id="c79e6-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="c79e6-112">[Configurar la aplicación en Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="c79e6-113">[Configurar la información de la aplicación](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="c79e6-114">[Configurar la configuración de la aplicación](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="c79e6-115">[Seleccionar las etiquetas de ámbito (opcional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="c79e6-116">[Agregar la aplicación](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="c79e6-117">Si necesita más ayuda, consulte [solución de problemas](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="c79e6-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




