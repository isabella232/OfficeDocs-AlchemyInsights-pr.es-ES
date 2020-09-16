---
title: Problemas relacionados con la VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726108"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="42715-102">Problemas relacionados con la VPN</span><span class="sxs-lookup"><span data-stu-id="42715-102">VPN related issues</span></span>

<span data-ttu-id="42715-103">La implementación correcta de conectividad VPN para los clientes MDM depende de un perfil implementado que refleja correctamente los requisitos de la infraestructura de VPN.</span><span class="sxs-lookup"><span data-stu-id="42715-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="42715-104">Para ver la configuración adecuada para las plataformas cliente que está investigando, vea:</span><span class="sxs-lookup"><span data-stu-id="42715-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="42715-105">Configuración de dispositivos de Windows 10 y Windows Holographic para agregar conexiones VPN con Intune</span><span class="sxs-lookup"><span data-stu-id="42715-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="42715-106">Agregar una configuración de VPN en dispositivos iOS y iPad en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="42715-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="42715-107">Configuración de dispositivo Android para configurar VPN en Intune</span><span class="sxs-lookup"><span data-stu-id="42715-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="42715-108">Agregar la configuración de VPN en los dispositivos macOS en Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="42715-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="42715-109">Si su perfil de VPN usa la autenticación basada en certificados, asegúrese de que el certificado raíz y los perfiles de certificación de autenticación de cliente vinculados al perfil de VPN se implementan correctamente.</span><span class="sxs-lookup"><span data-stu-id="42715-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="42715-110">**Problemas comunes**</span><span class="sxs-lookup"><span data-stu-id="42715-110">**Common Issues**</span></span>

<span data-ttu-id="42715-111">**Desplegó un perfil de VPN en un dispositivo. Intune muestra que se completó correctamente, pero el dispositivo no se conecta a la VPN.**</span><span class="sxs-lookup"><span data-stu-id="42715-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="42715-112">Un estado correcto significa que Intune ha implementado correctamente el perfil como configurado.</span><span class="sxs-lookup"><span data-stu-id="42715-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="42715-113">Sin embargo, estas configuraciones podrían no coincidir con los requisitos de red y/o autenticación.</span><span class="sxs-lookup"><span data-stu-id="42715-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="42715-114">Revisar registros en el servicio de autenticación y infraestructura (en el servidor VPN y en el servidor NPS/RADIUS) para más información sobre el intento de conexión.</span><span class="sxs-lookup"><span data-stu-id="42715-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="42715-115">Es posible que tenga que colaborar con el equipo de infraestructura de red o el proveedor de VPN de terceros para recopilar y revisar registros.</span><span class="sxs-lookup"><span data-stu-id="42715-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="42715-116">**Cuando configuro una VPN personalizada para iOS, la característica VPN por aplicación no está disponible.**</span><span class="sxs-lookup"><span data-stu-id="42715-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="42715-117">La VPN por aplicación para dispositivos iOS en Intune está actualmente disponible para una lista específica de proveedores y asociados, que también deben cumplir los requisitos previos de certificados antes de configurar una VPN por aplicación.</span><span class="sxs-lookup"><span data-stu-id="42715-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="42715-118">Para obtener más información, consulte [Configurar la red privada virtual (VPN) de cada aplicación para dispositivos iOS/iPad en Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="42715-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="42715-119">Para obtener más información acerca de todos los tipos de conexión VPN en Intune, consulte [Crear perfiles de VPN para conectarse a los servidores VPN en](https://docs.microsoft.com/intune/vpn-settings-configure)de Intune.</span><span class="sxs-lookup"><span data-stu-id="42715-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="42715-120">**La VPN a petición de iOS no se activa cuando se tiene acceso a un dominio configurado**</span><span class="sxs-lookup"><span data-stu-id="42715-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="42715-121">Para probar la configuración automática de VPN, configure los siguientes valores:</span><span class="sxs-lookup"><span data-stu-id="42715-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="42715-122">Quiero hacer lo siguiente: **Evaluar cada intento de conexión**</span><span class="sxs-lookup"><span data-stu-id="42715-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="42715-123">Elija si quiere conectar: **Conectar si es necesario**</span><span class="sxs-lookup"><span data-stu-id="42715-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="42715-124">Cuando los usuarios obtienen acceso a estos dominios: **de destino** *nombre de dominio*</span><span class="sxs-lookup"><span data-stu-id="42715-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="42715-125">Si la configuración anterior no se realiza correctamente, agregue el elemento siguiente:</span><span class="sxs-lookup"><span data-stu-id="42715-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="42715-126">Cuando no se puede tener acceso a esta dirección URL, obliga a conectar la red privada virtual: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="42715-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>