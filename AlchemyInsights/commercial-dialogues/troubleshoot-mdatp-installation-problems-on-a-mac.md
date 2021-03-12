---
title: Solucionar problemas de instalación de MDATP en un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737660"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="63ac8-102">Solucionar problemas de instalación de MDATP en un Mac</span><span class="sxs-lookup"><span data-stu-id="63ac8-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="63ac8-103">Si se produce un error en la instalación manual, la página **Resumen** del asistente para la instalación muestra el siguiente error:</span><span class="sxs-lookup"><span data-stu-id="63ac8-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="63ac8-104">"Se ha producido un error durante la instalación.</span><span class="sxs-lookup"><span data-stu-id="63ac8-104">"An error occurred during installation.</span></span> <span data-ttu-id="63ac8-105">El instalador encontró un error que provocó un error en la instalación.</span><span class="sxs-lookup"><span data-stu-id="63ac8-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="63ac8-106">Póngase en contacto con el fabricante del software para obtener ayuda."</span><span class="sxs-lookup"><span data-stu-id="63ac8-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="63ac8-107">Para las implementaciones de MDM, la página también muestra un error de instalación genérica.</span><span class="sxs-lookup"><span data-stu-id="63ac8-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="63ac8-108">Aunque no mostremos errores exactos a los usuarios finales, guardamos un archivo de registro con el progreso de la instalación, en **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="63ac8-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="63ac8-109">Cada sesión de instalación se anexa a este archivo de registro.</span><span class="sxs-lookup"><span data-stu-id="63ac8-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="63ac8-110">Para generar solo la última sesión de instalación, use `sed` .</span><span class="sxs-lookup"><span data-stu-id="63ac8-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="63ac8-111">Para obtener más información, vea [Solucionar problemas de instalación de ATP de Microsoft Defender para Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="63ac8-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
