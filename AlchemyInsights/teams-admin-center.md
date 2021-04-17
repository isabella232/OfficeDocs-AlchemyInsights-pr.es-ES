---
title: Centro de administración de Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826396"
---
# <a name="teams-admin-center"></a><span data-ttu-id="a1f6d-102">Centro de administración de Teams</span><span class="sxs-lookup"><span data-stu-id="a1f6d-102">Teams Admin Center</span></span>

<span data-ttu-id="a1f6d-103">Obtenga información acerca de cómo administrar Teams con el [Centro de administración de Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a1f6d-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="a1f6d-104">Si no puede acceder al Centro de administración de Teams, compruebe los siguientes elementos:</span><span class="sxs-lookup"><span data-stu-id="a1f6d-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="a1f6d-105">Compruebe que ha permitido las [direcciones IP y URL de Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) adecuadas en cualquier dispositivo perimetral (firewall, etc.) o en las reglas de firewall de su equipo local.</span><span class="sxs-lookup"><span data-stu-id="a1f6d-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="a1f6d-106">Compruebe que el inicio de sesión que usa para obtener acceso al Portal de administración de Teams coincide con el nombre de usuario que indicó en el [Portal de administración de Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a1f6d-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="a1f6d-107">Si los usuarios no aparecen en el Centro de administración de Teams, consulte lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="a1f6d-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="a1f6d-108">¿Ha creado usuarios o asignado licencias en las últimas 24 horas?</span><span class="sxs-lookup"><span data-stu-id="a1f6d-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="a1f6d-109">Asegúrese de que espera al menos 24 horas antes de abrir un vale de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="a1f6d-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="a1f6d-110">Compruebe que ha asignado las licencias adecuadas.</span><span class="sxs-lookup"><span data-stu-id="a1f6d-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="a1f6d-111">Si tiene un directorio local de Active Directory, compruebe que [el valor de msRTCSIP-PrimaryUserAddress o la dirección SIP en el campo ProxyAddresses de su Active Directory local es único y el formato coincide con](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) la sip:**nombre de usuario** del usuario del [Centro de administración de Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a1f6d-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="a1f6d-112">Si tiene previsto mantener una implementación de Skype Empresarial Server y hacer que los usuarios estén alojados de manera local y en línea, siga la **"Configuración híbrida con Teams y Skype Empresarial Online"** en el panel de control de Skype Empresarial Server y mueva a los usuarios en línea.</span><span class="sxs-lookup"><span data-stu-id="a1f6d-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
