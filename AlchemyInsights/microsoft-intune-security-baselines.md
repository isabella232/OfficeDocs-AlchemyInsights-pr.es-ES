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
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783227"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="edd5f-102">Usar Microsoft Intune de seguridad para configurar Windows 10 dispositivos</span><span class="sxs-lookup"><span data-stu-id="edd5f-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="edd5f-103">Las líneas base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="edd5f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="edd5f-104">Las líneas base de seguridad Windows los grupos preconfigurados que se usan para aplicar un grupo conocido de opciones y valores predeterminados recomendados por los equipos de seguridad relevantes.</span><span class="sxs-lookup"><span data-stu-id="edd5f-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="edd5f-105">Al crear un perfil de línea base de seguridad en Intune, crea una plantilla que consta de varios perfiles de configuración de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="edd5f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="edd5f-106">Al implementar líneas base de seguridad en grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o posterior.</span><span class="sxs-lookup"><span data-stu-id="edd5f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="edd5f-107">Por ejemplo, la línea base de seguridad de administración de dispositivos móviles (MDM) de Microsoft habilita automáticamente BitLocker para unidades extraíbles, requiere la contraseña para desbloquear un dispositivo y deshabilita la autenticación básica.</span><span class="sxs-lookup"><span data-stu-id="edd5f-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="edd5f-108">Cuando un valor predeterminado no funciona para su entorno, puede personalizar la línea base para aplicar la configuración que necesita.</span><span class="sxs-lookup"><span data-stu-id="edd5f-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="edd5f-109">Las líneas base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="edd5f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="edd5f-110">Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones de configuración que afectan a la seguridad.</span><span class="sxs-lookup"><span data-stu-id="edd5f-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="edd5f-111">Intune se asocia con el Windows de seguridad que crea líneas base para las directivas de grupo, por lo que estas recomendaciones se basan en una guía sólida y una amplia experiencia.</span><span class="sxs-lookup"><span data-stu-id="edd5f-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="edd5f-112">Si no conoce Intune y no sabe por dónde empezar, las líneas base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="edd5f-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="edd5f-113">Si actualmente usa una directiva de grupo, la migración a Intune con fines de administración es mucho más fácil con las líneas base de seguridad, ya que están integradas en Intune e incluyen funciones de administración de última generación.</span><span class="sxs-lookup"><span data-stu-id="edd5f-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="edd5f-114">Para obtener más información, [consulta Windows de seguridad y](/windows/security/threat-protection/windows-security-baselines) administración de [dispositivos móviles.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="edd5f-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

