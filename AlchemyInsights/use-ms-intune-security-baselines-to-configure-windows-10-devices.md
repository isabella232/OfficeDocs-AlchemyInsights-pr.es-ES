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
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="51f2c-102">Usar las líneas de base de seguridad de Microsoft Intune para configurar dispositivos Windows 10</span><span class="sxs-lookup"><span data-stu-id="51f2c-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="51f2c-103">Las líneas de base de seguridad de Intune ayudan a proteger a los usuarios y los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="51f2c-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="51f2c-104">Las líneas de base de seguridad son los grupos preconfigurados de Windows que se usan para aplicar un grupo conocido de valores de configuración y valores predeterminados recomendados por los equipos de seguridad correspondientes.</span><span class="sxs-lookup"><span data-stu-id="51f2c-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="51f2c-105">Mediante la creación de un perfil de línea base de seguridad en Intune, se crea una plantilla que consta de varios perfiles de configuración de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="51f2c-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="51f2c-106">Al implementar líneas de base de seguridad en grupos de usuarios o dispositivos, la configuración se aplica a los dispositivos que se ejecutan en Windows 10 o versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="51f2c-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="51f2c-107">Por ejemplo, la línea base de seguridad de MDM (1) habilita BitLocker para las unidades extraíbles, (2) requiere la contraseña para desbloquear un dispositivo y (3) deshabilita la autenticación básica.</span><span class="sxs-lookup"><span data-stu-id="51f2c-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="51f2c-108">Si un valor predeterminado no funciona en su entorno, personalice la línea de base para aplicar la configuración que necesita.</span><span class="sxs-lookup"><span data-stu-id="51f2c-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="51f2c-109">Las líneas de base de seguridad también ayudan a establecer un flujo de trabajo seguro de un extremo a otro en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="51f2c-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="51f2c-110">Estas son algunas de las ventajas de esto:</span><span class="sxs-lookup"><span data-stu-id="51f2c-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="51f2c-111">Una línea base de seguridad incluye los procedimientos recomendados y las recomendaciones para la configuración que afecta a la seguridad.</span><span class="sxs-lookup"><span data-stu-id="51f2c-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="51f2c-112">Como los asociados de Intune con el equipo de seguridad de Windows crean líneas de base para las directivas de grupo, estas recomendaciones se basan en una guía sólida y una amplia experiencia.</span><span class="sxs-lookup"><span data-stu-id="51f2c-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="51f2c-113">Si no está familiarizado con Intune y no está seguro de dónde empezar, las líneas de base de seguridad le ayudarán a crear e implementar rápidamente un perfil seguro.</span><span class="sxs-lookup"><span data-stu-id="51f2c-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="51f2c-114">Si actualmente usa una directiva de grupo, la migración a Intune para fines de administración es mucho más sencilla con las líneas de base de seguridad, ya que están integradas en Intune e incluyen capacidades de vanguardia para la administración.</span><span class="sxs-lookup"><span data-stu-id="51f2c-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="51f2c-115">Para obtener más información, consulte [Windows Security Baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="51f2c-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>