---
title: Usar las líneas base de seguridad de Microsoft Intune para configurar dispositivos con Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971536"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Usar las líneas base de seguridad de Microsoft Intune para configurar dispositivos con Windows 10

Las líneas base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos. Las líneas base de seguridad son grupos preconfigurados de la configuración de Windows que se usan para aplicar un grupo conocido de opciones de configuración y valores predeterminados recomendados por los equipos de seguridad correspondientes. Al crear un perfil de línea base de seguridad en Intune, crea una plantilla que consta de varios perfiles de configuración de dispositivos.

Al implementar líneas base de seguridad para grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o versiones posteriores. Por ejemplo, la línea base de seguridad de administración de dispositivos móviles (MDM) de Microsoft automáticamente (1) habilita BitLocker para unidades extraíbles, (2) requiere la contraseña para desbloquear un dispositivo y (3) deshabilita la autenticación básica. Cuando un valor predeterminado no funciona para su entorno, puede personalizar la línea base para aplicar la configuración que necesita.

Las líneas base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365. Estas son algunas de las ventajas de esta funcionalidad:
- Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones de configuración que afectan a la seguridad. Dado que Intune se asocia con el equipo de seguridad de Windows que crea líneas base para las directivas de grupo, estas recomendaciones se basan en una guía sólida y en una amplia experiencia.
- Si es nuevo en Intune y no está seguro de por dónde empezar, las líneas base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.
- Si usa actualmente una directiva de grupo, la migración a Intune con fines de administración es mucho más fácil con líneas base de seguridad, ya que estas líneas base de seguridad están integradas en Intune e incluyen funcionalidades avanzadas de administración.

Para más información, consulte [Líneas base de seguridad de Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) y [Administración de dispositivos móviles](https://docs.microsoft.com/windows/client-management/mdm/).