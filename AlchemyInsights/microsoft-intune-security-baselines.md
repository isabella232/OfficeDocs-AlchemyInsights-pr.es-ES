---
title: Usar Microsoft Intune de seguridad para configurar Windows 10 dispositivos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098079"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar Microsoft Intune de seguridad para configurar Windows 10 dispositivos

Las líneas base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos. Las líneas base de seguridad Windows los grupos preconfigurados que se usan para aplicar un grupo conocido de opciones y valores predeterminados recomendados por los equipos de seguridad relevantes. Al crear un perfil de línea base de seguridad en Intune, crea una plantilla que consta de varios perfiles de configuración de dispositivos.

Al implementar líneas base de seguridad en grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o posterior. Por ejemplo, la línea base de seguridad de administración de dispositivos móviles (MDM) de Microsoft habilita automáticamente BitLocker para unidades extraíbles, requiere la contraseña para desbloquear un dispositivo y deshabilita la autenticación básica. Cuando un valor predeterminado no funciona para su entorno, puede personalizar la línea base para aplicar la configuración que necesita.

Las líneas base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365. Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones de configuración que afectan a la seguridad. Intune se asocia con el Windows de seguridad que crea líneas base para las directivas de grupo, por lo que estas recomendaciones se basan en una guía sólida y una amplia experiencia.

Si no conoce Intune y no sabe por dónde empezar, las líneas base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro. Si actualmente usa una directiva de grupo, la migración a Intune con fines de administración es mucho más fácil con las líneas base de seguridad, ya que están integradas en Intune e incluyen funciones de administración de última generación.

Para obtener más información, [consulta Windows de seguridad y](/windows/security/threat-protection/windows-security-baselines) administración de [dispositivos móviles.](/windows/client-management/mdm/)

