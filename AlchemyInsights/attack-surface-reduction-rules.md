---
title: Reglas de reducción de la superficie expuesta a ataques
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651504"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="100ce-102">Reglas de reducción de la superficie expuesta a ataques</span><span class="sxs-lookup"><span data-stu-id="100ce-102">Attack surface reduction rules</span></span>

<span data-ttu-id="100ce-103">Excluir archivos o carpetas puede reducir considerablemente la protección proporcionada por las reglas de reducción de la superficie expuesta a ataques.</span><span class="sxs-lookup"><span data-stu-id="100ce-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="100ce-104">Esto permite ejecutar archivos que normalmente habrían sido bloqueados por una regla y no graba ningún informe o evento.</span><span class="sxs-lookup"><span data-stu-id="100ce-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="100ce-105">La exclusión se aplica a todas las reglas que permiten exclusiones.</span><span class="sxs-lookup"><span data-stu-id="100ce-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="100ce-106">Las exclusiones de ASR usan la misma sintaxis que las exclusiones de Antivirus de Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="100ce-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="100ce-107">Para obtener más información, consulte [Configurar y validar exclusiones para el análisis de Antivirus de Microsoft Defender](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="100ce-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="100ce-108">Para evitar problemas, revise los [Errores comunes que puede evitar al definir las exclusiones](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="100ce-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="100ce-109">No todas las reglas de ASR admiten exclusiones.</span><span class="sxs-lookup"><span data-stu-id="100ce-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="100ce-110">Para comprobar si la regla admite exclusiones, vea la tabla [Reglas de reducción de la superficie expuesta a ataques](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="100ce-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="100ce-111">Reglas de reducción de la superficie expuesta a ataques</span><span class="sxs-lookup"><span data-stu-id="100ce-111">Attack surface reduction rules</span></span>

<span data-ttu-id="100ce-112">En la superficie de ataque de la organización se incluyen todos los lugares a través de los cuales un atacante podría poner en peligro a los dispositivos o las redes de la organización.</span><span class="sxs-lookup"><span data-stu-id="100ce-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="100ce-113">Reducir la superficie expuesta a ataques implica proteger los dispositivos y la red de la organización, lo cual limita a los atacantes las formas de realizar el ataque.</span><span class="sxs-lookup"><span data-stu-id="100ce-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="100ce-114">Configurar reglas de reducción de la superficie expuesta a ataques en Microsoft Defender para punto de conexión puede ayudarle.</span><span class="sxs-lookup"><span data-stu-id="100ce-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="100ce-115">Para más información, consulte:</span><span class="sxs-lookup"><span data-stu-id="100ce-115">For more information, see:</span></span>

- [<span data-ttu-id="100ce-116">Asignar GUID de regla de ASR al nombre</span><span class="sxs-lookup"><span data-stu-id="100ce-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="100ce-117">Requisitos de reglas de ASR:</span><span class="sxs-lookup"><span data-stu-id="100ce-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="100ce-118">Windows 10 Pro, versión 1709 o posterior</span><span class="sxs-lookup"><span data-stu-id="100ce-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="100ce-119">Windows 10 Enterprise, versión 1709 o posterior</span><span class="sxs-lookup"><span data-stu-id="100ce-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="100ce-120">Windows Server, versión 1803 (Canal semestral) o posterior</span><span class="sxs-lookup"><span data-stu-id="100ce-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="100ce-121">Identificar la exclusión correcta que se aplicará</span><span class="sxs-lookup"><span data-stu-id="100ce-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="100ce-122">Busque eventID 1121 o 1122 en el registro Microsoft-Windows-Windows Defender/Registro operativo.</span><span class="sxs-lookup"><span data-stu-id="100ce-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="100ce-123">Evalúe el escenario y el contexto del bloque y confirme que es necesario desbloquear este escenario.</span><span class="sxs-lookup"><span data-stu-id="100ce-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="100ce-124">Lea el valor de la ruta de acceso en los detalles del evento, que es el valor que define la exclusión.</span><span class="sxs-lookup"><span data-stu-id="100ce-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="100ce-125">Haga que la exclusión sea lo más estricta posible.</span><span class="sxs-lookup"><span data-stu-id="100ce-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="100ce-126">Aplique un carácter comodín según sea necesario (por ejemplo, reemplace la variable de usuario).</span><span class="sxs-lookup"><span data-stu-id="100ce-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="100ce-127">Aplique la exclusión según las necesidades de implementación.</span><span class="sxs-lookup"><span data-stu-id="100ce-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="100ce-128">Para obtener más información, consulte [Personalizar las reglas de reducción de la superficie expuesta a ataques](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="100ce-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="100ce-129">No se respeta la exclusión</span><span class="sxs-lookup"><span data-stu-id="100ce-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="100ce-130">Determine si la regla admite exclusiones.</span><span class="sxs-lookup"><span data-stu-id="100ce-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="100ce-131">Para obtener más información, consulte [Reglas de reducción de la superficie expuesta a ataques](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="100ce-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="100ce-132">Revise las exclusiones aplicadas y compruebe con los datos del evento si hay errores tipográficos o caracteres comodín que no se hayan podido interpretar.</span><span class="sxs-lookup"><span data-stu-id="100ce-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="100ce-133">Para obtener más información, consulte [Tipos de exclusión admitidos](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="100ce-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="100ce-134">Si el impacto de la regla es demasiado alto, considere la posibilidad de mover la regla (de vuelta) al modo de Auditoría para una validación adicional.</span><span class="sxs-lookup"><span data-stu-id="100ce-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="100ce-135">Para obtener más información, consulte [Probar cómo funcionan las características de Microsoft Defender para punto de conexión en modo de auditoría](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="100ce-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="100ce-136">Recopile los datos de soporte técnico para abrir un caso de soporte con este comando:</span><span class="sxs-lookup"><span data-stu-id="100ce-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="100ce-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="100ce-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="100ce-138">Para obtener más información, consulte [Problemas de incorporación de equipos a Microsoft Defender para punto de conexión](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="100ce-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
