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
ms.openlocfilehash: f7811c15af21d8e7790e6686bb8ba9e5de3659d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319013"
---
# <a name="attack-surface-reduction-rules"></a>Reglas de reducción de la superficie expuesta a ataques

Excluir archivos o carpetas puede reducir considerablemente la protección proporcionada por las reglas de reducción de la superficie expuesta a ataques. Esto permite ejecutar archivos que normalmente habrían sido bloqueados por una regla y no graba ningún informe o evento. La exclusión se aplica a todas las reglas que permiten exclusiones.

Las exclusiones de ASR usan la misma sintaxis que las exclusiones de Antivirus de Microsoft Defender. Para obtener más información, consulte [Configurar y validar exclusiones para el análisis de Antivirus de Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Para evitar problemas, revise los [Errores comunes que puede evitar al definir las exclusiones](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

No todas las reglas de ASR admiten exclusiones. Para comprobar si la regla admite exclusiones, vea la tabla [Reglas de reducción de la superficie expuesta a ataques](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Reglas de reducción de la superficie expuesta a ataques

En la superficie de ataque de la organización se incluyen todos los lugares a través de los cuales un atacante podría poner en peligro a los dispositivos o las redes de la organización. Reducir la superficie expuesta a ataques implica proteger los dispositivos y la red de la organización, lo cual limita a los atacantes las formas de realizar el ataque. Configurar reglas de reducción de la superficie expuesta a ataques en Microsoft Defender para punto de conexión puede ayudarle.

Para más información, consulte:

- [Asignar GUID de regla de ASR al nombre](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Requisitos de reglas de ASR:
    - [Windows 10 Pro, versión 1709 o posterior](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versión 1709 o posterior](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versión 1803 (Canal semestral) o posterior](https://docs.microsoft.com/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificar la exclusión correcta que se aplicará

1. Busque eventID 1121 o 1122 en el registro Microsoft-Windows-Windows Defender/Registro operativo.

1. Evalúe el escenario y el contexto del bloque y confirme que es necesario desbloquear este escenario.

1. Lea el valor de la ruta de acceso en los detalles del evento, que es el valor que define la exclusión.
    - Haga que la exclusión sea lo más estricta posible.
    - Aplique un carácter comodín según sea necesario (por ejemplo, reemplace la variable de usuario).

1. Aplique la exclusión según las necesidades de implementación. Para obtener más información, consulte [Personalizar las reglas de reducción de la superficie expuesta a ataques](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>No se respeta la exclusión

1. Determine si la regla admite exclusiones. Para obtener más información, consulte [Reglas de reducción de la superficie expuesta a ataques](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Revise las exclusiones aplicadas y compruebe con los datos del evento si hay errores tipográficos o caracteres comodín que no se hayan podido interpretar. Para obtener más información, consulte [Tipos de exclusión admitidos](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Si el impacto de la regla es demasiado alto, considere la posibilidad de mover la regla (de vuelta) al modo de Auditoría para una validación adicional. Para obtener más información, consulte [Probar cómo funcionan las características de Microsoft Defender para punto de conexión en modo de auditoría](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Recopile los datos de soporte técnico para abrir un caso de soporte con este comando:
    
   ** MDEClientAnalyzer.cmd -v**

    Para obtener más información, consulte [Problemas de incorporación de equipos a Microsoft Defender para punto de conexión](issues-with-onboarding-machines.md).
