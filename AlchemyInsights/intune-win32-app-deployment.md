---
title: Implementación de aplicaciones Win32 de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366551"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="a8c16-102">Implementación de aplicaciones Win32 de Intune</span><span class="sxs-lookup"><span data-stu-id="a8c16-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="a8c16-103">Microsoft Intune permite que las aplicaciones Win32, como MSI y .EXE, se implementen en dispositivos con Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a8c16-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="a8c16-104">El mecanismo de implementación utilizado requiere que la Extensión de administración de Intune (IME) esté presente en el dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="a8c16-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="a8c16-105">El IME se instalará automáticamente como resultado de la selección de una implementación de script de PowerShell o de una aplicación Win32 en un usuario o dispositivo.  </span><span class="sxs-lookup"><span data-stu-id="a8c16-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="a8c16-106">También hay un conjunto de requisitos previos que deben cumplirse para poder implementar aplicaciones Win32, entre los que se incluyen:</span><span class="sxs-lookup"><span data-stu-id="a8c16-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="a8c16-107">Plataformas compatibles: Windows 10 versión 1607 o posterior (versiones Enterprise, Pro y Education).</span><span class="sxs-lookup"><span data-stu-id="a8c16-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="a8c16-108">Arquitectura compatible: x86 y x64.</span><span class="sxs-lookup"><span data-stu-id="a8c16-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="a8c16-109">Administración de dispositivos: AAD unido e inscrito automáticamente (incluido el dominio híbrido unido y la directiva de grupo inscrita automáticamente)</span><span class="sxs-lookup"><span data-stu-id="a8c16-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="a8c16-110">Formato de paquete de la aplicación: archivo .**intunewin** preparado por la [Herramienta de preparación de contenido de Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="a8c16-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="a8c16-111">Limitaciones:</span><span class="sxs-lookup"><span data-stu-id="a8c16-111">Limitations:</span></span>
    - <span data-ttu-id="a8c16-112">Tamaño máximo: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="a8c16-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="a8c16-113">Arquitectura no compatible: ARM.</span><span class="sxs-lookup"><span data-stu-id="a8c16-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="a8c16-114">Revise el documento "[Agregar, asignar y supervisar una aplicación Win32 en Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" para información relacionada con estos pasos.</span><span class="sxs-lookup"><span data-stu-id="a8c16-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="a8c16-115">Los detalles sobre la implementación de aplicaciones de resolución de problemas en Windows, incluidas las aplicaciones Win32, se pueden revisar en los siguientes documentos</span><span class="sxs-lookup"><span data-stu-id="a8c16-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="a8c16-116">Solución de problemas de instalación de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="a8c16-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="a8c16-117">Solución de problemas de aplicaciones de Win32</span><span class="sxs-lookup"><span data-stu-id="a8c16-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)