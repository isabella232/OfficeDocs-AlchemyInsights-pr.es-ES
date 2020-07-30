---
title: Usar perfiles de correo electrónico con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505237"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="ae30a-102">Usar perfiles de correo electrónico con Intune</span><span class="sxs-lookup"><span data-stu-id="ae30a-102">Using email profiles with Intune</span></span>

<span data-ttu-id="ae30a-103">Intune se puede usar para crear e implementar perfiles de correo electrónico para el cliente de correo electrónico nativo (integrado) en varias plataformas de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ae30a-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="ae30a-104">Para más información sobre algunas de las restricciones relacionadas con los perfiles de correo electrónico, como la forma en que se controlan la presencia de los perfiles existentes y cómo quitar los perfiles de correo electrónico, consulte [Agregar la configuración de correo electrónico en dispositivos con Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="ae30a-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="ae30a-105">Para obtener más información acerca de cómo crear perfiles de correo electrónico para cada plataforma de dispositivo, consulte:</span><span class="sxs-lookup"><span data-stu-id="ae30a-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="ae30a-106">Configuración de dispositivo Android para configurar el correo electrónico, la autenticación y la sincronización en Intune</span><span class="sxs-lookup"><span data-stu-id="ae30a-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="ae30a-107">Agregar la configuración de correo electrónico para dispositivos iOS y iPadOS en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ae30a-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="ae30a-108">Configuración del perfil de correo electrónico en Microsoft Intune para dispositivos que ejecutan Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="ae30a-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="ae30a-109">Configuración de Perfil de correo electrónico para dispositivos que ejecutan Windows 10 en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ae30a-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="ae30a-110">**Problema común de sincronización**</span><span class="sxs-lookup"><span data-stu-id="ae30a-110">**Common syncing issue**</span></span>

<span data-ttu-id="ae30a-111">**Un perfil de correo electrónico KNOX on Android impide que los contactos, el Calendario de Outlook y las tareas de usuario se sincronicen con los dispositivos de usuario.**</span><span class="sxs-lookup"><span data-stu-id="ae30a-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="ae30a-112">El perfil de correo electrónico KNOX on Android KNOX ofrece al administrador la opción de decidir qué tipos de contenido se sincronizan con el dispositivo al establecer cada uno en enabled.</span><span class="sxs-lookup"><span data-stu-id="ae30a-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="ae30a-113">Si la configuración de cualquiera de los tipos de contenido se establece en **No se configura** (predeterminado), el tipo de contenido no se sincronizará automáticamente.</span><span class="sxs-lookup"><span data-stu-id="ae30a-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="ae30a-114">Es posible que un usuario habilite el tipo de contenido que quiera directamente en el dispositivo de forma manual, pero que la configuración de directiva de Intune sobrescriba la configuración y se detenga la sincronización de ese tipo de contenido.</span><span class="sxs-lookup"><span data-stu-id="ae30a-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

