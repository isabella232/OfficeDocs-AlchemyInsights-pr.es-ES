---
title: Usar Microsoft Intune de seguridad para configurar Windows 10 dispositivos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104361"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar Microsoft Intune de seguridad para configurar Windows 10 dispositivos

Las líneas base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos. Las líneas base de seguridad son grupos preconfigurados de la configuración de Windows que se usan para aplicar un grupo conocido de opciones de configuración y valores predeterminados recomendados por los equipos de seguridad correspondientes. Al crear un perfil de línea base de seguridad en Intune, crea una plantilla que consta de varios perfiles de configuración de dispositivos.

Al implementar líneas base de seguridad en grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o posterior. Por ejemplo, mdm security baseline automáticamente (1) habilita BitLocker para unidades extraíbles, (2) requiere la contraseña para desbloquear un dispositivo y (3) deshabilita la autenticación básica. Cuando un valor predeterminado no funciona para el entorno, personalice la línea base para aplicar la configuración que necesita.

Las líneas base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365. Estas son algunas de las ventajas de esto:

- Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones de configuración que afectan a la seguridad. Dado que Intune se asocia con el equipo de seguridad de Windows que crea líneas base para las directivas de grupo, estas recomendaciones se basan en una guía sólida y en una amplia experiencia.
- Si es nuevo en Intune y no está seguro de por dónde empezar, las líneas base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.
- Si actualmente usa una directiva de grupo, la migración a Intune con fines de administración es mucho más fácil con las líneas base de seguridad, ya que están integradas en Intune e incluyen funciones de última generación para la administración.

Para obtener más información, [consulta Windows de seguridad y](https://go.microsoft.com/fwlink/?linkid=2141503) administración de [dispositivos móviles.](https://go.microsoft.com/fwlink/?linkid=2141701)