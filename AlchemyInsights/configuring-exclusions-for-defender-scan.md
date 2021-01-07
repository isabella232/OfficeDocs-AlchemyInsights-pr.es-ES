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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768489"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="4a649-102">Configurar exclusiones para el análisis de ATP de Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="4a649-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="4a649-103">En general, puede excluir ciertas extensiones de archivo y ubicaciones de carpeta de los análisis de ATP de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="4a649-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="4a649-104">Asimismo, puede configurar exclusiones para los archivos abiertos por ciertos procesos.</span><span class="sxs-lookup"><span data-stu-id="4a649-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="4a649-105">Para más información, consulte [Configurar y validar exclusiones en función de la extensión del archivo y la ubicación de la carpeta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) y [Configurar exclusiones para archivos abiertos por procesos](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="4a649-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="4a649-106">Para configurar exclusiones para **Windows Server 2016 y 2019**, consulte [Configurar exclusiones del Antivirus de Microsoft Defender en Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="4a649-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="4a649-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="4a649-107">**Mac**</span></span>

<span data-ttu-id="4a649-108">Para más detalles sobre los tipos de exclusión admitidos y configurar una lista de exclusiones para Mac, consulte [Tipos de exclusión admitidos](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) y [Cómo configurar la lista de exclusiones](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="4a649-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="4a649-109">**Nota** También puede validar las listas de exclusiones mediante el archivo de prueba de EICAR.</span><span class="sxs-lookup"><span data-stu-id="4a649-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="4a649-110">Para más información, consulte [Validar las listas de exclusiones mediante el archivo de prueba de EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="4a649-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="4a649-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="4a649-111">**Linux**</span></span>

<span data-ttu-id="4a649-112">Para más detalles sobre los tipos de exclusión admitidos y configurar una lista de exclusiones para Linux, consulte [Tipos de exclusión admitidos](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) y [Configurar y validar exclusiones para ATP de Microsoft Defender para Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="4a649-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="4a649-113">**Nota** También puede validar las listas de exclusiones mediante el archivo de prueba de EICAR.</span><span class="sxs-lookup"><span data-stu-id="4a649-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="4a649-114">Para más información, consulte [Validar las listas de exclusiones mediante el archivo de prueba de EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="4a649-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 