---
title: Solución de problemas de implementación de certificados de autenticación de cliente
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659003"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="2478d-102">Solución de problemas de implementación de certificados de autenticación de cliente</span><span class="sxs-lookup"><span data-stu-id="2478d-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="2478d-103">Los perfiles de certificados de cliente de Intune NDES/SCEP y PKCS/PFX suelen usarse en combinación con otros tipos de perfiles, como WiFi, VPN y correo electrónico, para permitir que los usuarios puedan autenticarse en los recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="2478d-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="2478d-104">Cuando estos tipos de perfil están vinculados a un perfil de certificado de cliente dependen de la implementación correcta de este perfil.</span><span class="sxs-lookup"><span data-stu-id="2478d-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="2478d-105">La configuración inicial de la infraestructura y la configuración asociada del perfil de certificado del cliente a menudo necesitan solucionar un problema.</span><span class="sxs-lookup"><span data-stu-id="2478d-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="2478d-106">Para obtener una guía paso a paso para configurar correctamente el conector NDES y las instrucciones para la solución de problemas para aislar problemas con la implementación de certificados, vea:</span><span class="sxs-lookup"><span data-stu-id="2478d-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="2478d-107">Configurar la infraestructura de para admitir SCEP con Intune</span><span class="sxs-lookup"><span data-stu-id="2478d-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- <span data-ttu-id="2478d-108">[Información general sobre la solución de problemas de perfiles de certificado SCEP con Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2478d-108">[Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)</span></span>

<span data-ttu-id="2478d-109">Use los scripts de PowerShell a los que se hace referencia para ayudar a comprobar la configuración.</span><span class="sxs-lookup"><span data-stu-id="2478d-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="2478d-110">Para obtener más información, consulte [Scripts de Verificación de conectores de Certificados de Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="2478d-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="2478d-111">**Otros problemas comunes**</span><span class="sxs-lookup"><span data-stu-id="2478d-111">**Other common issues**</span></span>

<span data-ttu-id="2478d-112">**Cuando intento instalar el conector de certificados de Intune en el servidor de conectores de NDES, recibo el mensaje "no se puede comprobar la contraseña de la solicitud de certificado". Es posible que ya se haya usado. Obtenga una nueva contraseña para enviar con esta solicitud ".**</span><span class="sxs-lookup"><span data-stu-id="2478d-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="2478d-113">Este mensaje quiere decir que debe ejecutar la instalación de conector de certificados como administrador.</span><span class="sxs-lookup"><span data-stu-id="2478d-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="2478d-114">En algunos entornos, los servidores en los que se ejecuta el certificado de Intune deben usar un servidor proxy para conectarse a Intune y, por lo tanto, el conector de certificados debe usar un proxy.</span><span class="sxs-lookup"><span data-stu-id="2478d-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="2478d-115">En algunos casos, NDES Connector omite la configuración de proxy configurada y puede que sea necesario configurar la configuración de proxy mientras se ejecuta en el contexto de seguridad de LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="2478d-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="2478d-116">La solución consiste en ejecutar Internet Explorer como SYSTEM y configurar un servidor proxy en IE.</span><span class="sxs-lookup"><span data-stu-id="2478d-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="2478d-117">Después de reiniciar el servicio del conector Intune, el conector NDES se conecta a Intune.</span><span class="sxs-lookup"><span data-stu-id="2478d-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="2478d-118">**Los dispositivos de los usuarios ya no reciben certificados SCEP de NDES.**</span><span class="sxs-lookup"><span data-stu-id="2478d-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="2478d-119">Es posible que el certificado de autenticación de cliente emitido al servidor NDES y que se especifica durante la instalación de NDES Connector, haya expirado o no se encuentra.</span><span class="sxs-lookup"><span data-stu-id="2478d-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="2478d-120">Para resolver:</span><span class="sxs-lookup"><span data-stu-id="2478d-120">To resolve:</span></span> 
 
1. <span data-ttu-id="2478d-121">Desinstale el conector NDES.</span><span class="sxs-lookup"><span data-stu-id="2478d-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="2478d-122">Use estos detalles para solicitar una nueva autenticación de cliente o certificado de autenticación de servidor:</span><span class="sxs-lookup"><span data-stu-id="2478d-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="2478d-123">Nombre de firmante: CN=FQDN externo</span><span class="sxs-lookup"><span data-stu-id="2478d-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="2478d-124">Nombre alternativo del firmante (se requieren ambos): DNS = FQDN externo, DNS=FQDN interno</span><span class="sxs-lookup"><span data-stu-id="2478d-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="2478d-125">Vuelva a instalar el conector NDES con el nuevo certificado.</span><span class="sxs-lookup"><span data-stu-id="2478d-125">Reinstall the NDES connector with the new certificate.</span></span>