---
title: Perfiles de Wi-Fi de Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696278"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="d9a63-102">Perfiles de Wi-Fi de Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="d9a63-103">La implementación correcta de conectividad Wi-Fi para los clientes MDM depende de un perfil correctamente implementado que refleja los requisitos de la infraestructura de Wi-Fi corporativa.</span><span class="sxs-lookup"><span data-stu-id="d9a63-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="d9a63-104">Para revisar la configuración adecuada para las plataformas de cliente que está investigando, consulte:</span><span class="sxs-lookup"><span data-stu-id="d9a63-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="d9a63-105">Agregar la configuración de Wi-Fi para dispositivos que ejecutan Android en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="d9a63-106">Agregar la configuración de Wi-Fi para dispositivos Android Enterprise dedicados y totalmente administrados en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="d9a63-107">Agregar la configuración de Wi-Fi para dispositivos iOS e iPadOS en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="d9a63-108">Agregar la configuración de Wi-Fi para dispositivos con Windows 10 y versiones posteriores en Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="d9a63-109">Importar la configuración de Wi-Fi para dispositivos con Windows en Intune</span><span class="sxs-lookup"><span data-stu-id="d9a63-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="d9a63-110">**Problemas comunes**</span><span class="sxs-lookup"><span data-stu-id="d9a63-110">**Common Issues**</span></span>

<span data-ttu-id="d9a63-111">**Estoy implementando un perfil de Wi-Fi que depende de un certificado implementado especificado en el perfil de Wi-Fi. Sin embargo, los perfiles de configuración muestran un estado de error.**</span><span class="sxs-lookup"><span data-stu-id="d9a63-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="d9a63-112">Compruebe la recepción del certificado en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9a63-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="d9a63-113">En Intune, vaya a **Todos los dispositivos** y seleccione el dispositivo > **Configuración del dispositivo**.</span><span class="sxs-lookup"><span data-stu-id="d9a63-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="d9a63-114">Compruebe que todos los perfiles previstos estén enumerados y en un estado correcto.</span><span class="sxs-lookup"><span data-stu-id="d9a63-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="d9a63-115">Para un perfil Android, si tiene certificados intermedios en la cadena de certificados, asegúrese de que se implementen en dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="d9a63-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="d9a63-116">Para comprobar el estado del certificado, vaya a **Configuración del dispositivo** > **Perfiles** > **Entidad de certificación intermedio de Android** > **Propiedades** > **Certificado de confianza**.</span><span class="sxs-lookup"><span data-stu-id="d9a63-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="d9a63-117">Si aún observa errores, revise los procedimientos y las secciones de solución de problemas.</span><span class="sxs-lookup"><span data-stu-id="d9a63-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="d9a63-118">Para obtener más información, consulte [Información general sobre la solución de problemas de perfiles de certificado SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d9a63-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="d9a63-119">**Desplegó un perfil de Wi-Fi en un dispositivo. Intune muestra que se completó correctamente, pero el dispositivo no se conecta al Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="d9a63-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="d9a63-120">Un estado correcto significa que Intune ha implementado correctamente el perfil como configurado.</span><span class="sxs-lookup"><span data-stu-id="d9a63-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="d9a63-121">Sin embargo, estas configuraciones podrían no coincidir con los requisitos de red y/o autenticación.</span><span class="sxs-lookup"><span data-stu-id="d9a63-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="d9a63-122">Para más información sobre el intento de conexión, revise los registros en el servicio de autenticación e infraestructura (en el controlador del punto de acceso Wi-Fi y el servidor NPS/RADIUS).</span><span class="sxs-lookup"><span data-stu-id="d9a63-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="d9a63-123">Es posible que tenga que colaborar con el equipo de infraestructura de red o el proveedor de Wi-Fi de terceros para recopilar y revisar registros.</span><span class="sxs-lookup"><span data-stu-id="d9a63-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>