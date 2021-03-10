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
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641628"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="ddec1-102">Usar las líneas base de seguridad de Microsoft Intune para configurar dispositivos con Windows 10</span><span class="sxs-lookup"><span data-stu-id="ddec1-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="ddec1-103">Las líneas base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ddec1-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ddec1-104">Las líneas base de seguridad son grupos preconfigurados de la configuración de Windows que se usan para aplicar un grupo conocido de opciones de configuración y valores predeterminados recomendados por los equipos de seguridad correspondientes.</span><span class="sxs-lookup"><span data-stu-id="ddec1-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ddec1-105">Al crear un perfil de línea base de seguridad en Intune, crea una plantilla que consta de varios perfiles de configuración de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ddec1-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ddec1-106">Al implementar líneas base de seguridad para grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="ddec1-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="ddec1-107">Por ejemplo, la línea base de seguridad de administración de dispositivos móviles (MDM) de Microsoft automáticamente (1) habilita BitLocker para unidades extraíbles, (2) requiere la contraseña para desbloquear un dispositivo y (3) deshabilita la autenticación básica.</span><span class="sxs-lookup"><span data-stu-id="ddec1-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ddec1-108">Cuando un valor predeterminado no funciona para su entorno, puede personalizar la línea base para aplicar la configuración que necesita.</span><span class="sxs-lookup"><span data-stu-id="ddec1-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ddec1-109">Las líneas base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ddec1-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ddec1-110">Estas son algunas de las ventajas de esta funcionalidad:</span><span class="sxs-lookup"><span data-stu-id="ddec1-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="ddec1-111">Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones de configuración que afectan a la seguridad.</span><span class="sxs-lookup"><span data-stu-id="ddec1-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ddec1-112">Dado que Intune se asocia con el equipo de seguridad de Windows que crea líneas base para las directivas de grupo, estas recomendaciones se basan en una guía sólida y en una amplia experiencia.</span><span class="sxs-lookup"><span data-stu-id="ddec1-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ddec1-113">Si es nuevo en Intune y no está seguro de por dónde empezar, las líneas base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="ddec1-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ddec1-114">Si usa actualmente una directiva de grupo, la migración a Intune con fines de administración es mucho más fácil con líneas base de seguridad, ya que estas líneas base de seguridad están integradas en Intune e incluyen funcionalidades avanzadas de administración.</span><span class="sxs-lookup"><span data-stu-id="ddec1-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ddec1-115">Para más información, consulte [Líneas base de seguridad de Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) y [Administración de dispositivos móviles](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="ddec1-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>