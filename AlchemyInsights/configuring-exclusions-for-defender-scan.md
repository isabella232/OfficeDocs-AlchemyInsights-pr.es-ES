---
title: Configurar exclusiones para el análisis de ATP de Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543702"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="8d3bd-102">Configurar exclusiones para el análisis de ATP de Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="8d3bd-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="8d3bd-103">En general, puede excluir ciertas extensiones de archivo y ubicaciones de carpeta de los análisis de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="8d3bd-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="8d3bd-104">Asimismo, puede configurar exclusiones para los archivos abiertos por ciertos procesos.</span><span class="sxs-lookup"><span data-stu-id="8d3bd-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="8d3bd-105">Para más información, consulte [Configurar y validar exclusiones en función de la extensión del archivo y la ubicación de la carpeta](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) y [Configurar exclusiones para archivos abiertos por procesos](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="8d3bd-106">Para configurar exclusiones para **Windows Server 2016 y 2019**, consulte [Configurar exclusiones del Antivirus de Microsoft Defender en Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="8d3bd-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="8d3bd-107">**Mac**</span></span>

<span data-ttu-id="8d3bd-108">Para más detalles sobre los tipos de exclusión admitidos y configurar una lista de exclusiones para Mac, consulte [Tipos de exclusión admitidos](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) y [Cómo configurar la lista de exclusiones](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="8d3bd-109">**Nota** También puede validar las listas de exclusiones mediante el archivo de prueba de EICAR.</span><span class="sxs-lookup"><span data-stu-id="8d3bd-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="8d3bd-110">Para más información, consulte [Validar las listas de exclusiones mediante el archivo de prueba de EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="8d3bd-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="8d3bd-111">**Linux**</span></span>

<span data-ttu-id="8d3bd-112">Para más detalles sobre los tipos de exclusión admitidos y configurar una lista de exclusiones para Linux, consulte [Tipos de exclusión admitidos](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) y [Configurar y validar exclusiones para ATP de Microsoft Defender para Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="8d3bd-113">**Nota** También puede validar las listas de exclusiones mediante el archivo de prueba de EICAR.</span><span class="sxs-lookup"><span data-stu-id="8d3bd-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="8d3bd-114">Para más información, consulte [Validar las listas de exclusiones mediante el archivo de prueba de EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="8d3bd-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 