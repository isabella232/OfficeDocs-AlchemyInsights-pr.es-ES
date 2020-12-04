---
title: Usar las líneas de base de seguridad de Microsoft Intune para configurar dispositivos Windows 10
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
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571894"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usar las líneas de base de seguridad de Microsoft Intune para configurar dispositivos Windows 10

Las líneas de base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos. Las líneas de base de seguridad son los grupos preconfigurados de Windows que se usan para aplicar un grupo conocido de valores de configuración y valores predeterminados recomendados por los equipos de seguridad correspondientes. Mediante la creación de un perfil de línea base de seguridad en Intune, se crea una plantilla que consta de varios perfiles de configuración de dispositivos.

Al implementar líneas de base de seguridad en grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o versiones posteriores. Por ejemplo, la línea base de seguridad de MDM (1) habilita BitLocker para las unidades extraíbles, (2) requiere la contraseña para desbloquear un dispositivo y (3) deshabilita la autenticación básica. Si un valor predeterminado no funciona en su entorno, personalice la línea de base para aplicar la configuración que necesita.

Las líneas de base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365. Estas son algunas de las ventajas de esto:

- Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones para la configuración que afecta a la seguridad. Como los asociados de Intune con el equipo de seguridad de Windows crean líneas de base para las directivas de grupo, estas recomendaciones se basan en una guía sólida y una amplia experiencia.
- Si no está familiarizado con Intune y no está seguro de dónde empezar, las líneas de base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.
- Si actualmente usa una directiva de grupo, la migración a Intune para fines de administración es mucho más sencilla con las líneas de base de seguridad, ya que están integradas en Intune e incluyen capacidades de vanguardia para la administración.

Para obtener más información, consulte [Windows Security Baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).