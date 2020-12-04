---
title: Solucionar un problema de PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571973"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="89916-102">Solucionar un problema de PRT</span><span class="sxs-lookup"><span data-stu-id="89916-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="89916-103">Para que cualquier dispositivo finalice su autenticación, debe estar completamente registrado y en buen estado y poder adquirir un token de actualización principal (PRT).</span><span class="sxs-lookup"><span data-stu-id="89916-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="89916-104">El proceso de registro de Unión híbrida de Azure AD requiere que los dispositivos estén en una red corporativa.</span><span class="sxs-lookup"><span data-stu-id="89916-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="89916-105">También funciona con VPN, pero hay algunas advertencias.</span><span class="sxs-lookup"><span data-stu-id="89916-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="89916-106">Hemos escuchado a los clientes que necesitan asistencia para solucionar problemas del proceso de registro de Unión híbrida de Azure AD en circunstancias laborales remotas.</span><span class="sxs-lookup"><span data-stu-id="89916-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="89916-107">A continuación, se muestra un desglose de lo que sucede ' en el parasol ' durante el proceso de registro.</span><span class="sxs-lookup"><span data-stu-id="89916-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="89916-108">**Entorno de autenticación en la nube (mediante la sincronización de hash de contraseña de Azure AD o la autenticación de paso a través)**</span><span class="sxs-lookup"><span data-stu-id="89916-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="89916-109">Este flujo de registro también se conoce como "sincronización de sincronización".</span><span class="sxs-lookup"><span data-stu-id="89916-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="89916-110">Windows 10 descubre un registro SCP cuando el usuario inicia sesión en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89916-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="89916-111">En primer lugar, el dispositivo intenta recuperar información de inquilinos del SCP del lado cliente en el registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="89916-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="89916-112">Para obtener más información, vea este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="89916-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="89916-113">Si se produce un error, el dispositivo se comunica con Active Directory local (AD) para obtener la información de inquilino del punto de conexión de servicio (SCP).</span><span class="sxs-lookup"><span data-stu-id="89916-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="89916-114">Para comprobar el SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="89916-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="89916-115">Se recomienda habilitar SCP en AD y usar el SCP del lado cliente para la validación inicial.</span><span class="sxs-lookup"><span data-stu-id="89916-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="89916-116">Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD.</span><span class="sxs-lookup"><span data-stu-id="89916-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="89916-117">Puede comprobar si el dispositivo puede tener acceso a los recursos de Microsoft en la cuenta del sistema mediante el script de conectividad de registro de dispositivos de prueba.</span><span class="sxs-lookup"><span data-stu-id="89916-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="89916-118">Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en AD local.</span><span class="sxs-lookup"><span data-stu-id="89916-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="89916-119">Esto requiere línea de vista a controlador de dominio.</span><span class="sxs-lookup"><span data-stu-id="89916-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="89916-120">Un objeto de dispositivo que tiene un certificado se sincroniza con Azure AD a través de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="89916-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="89916-121">El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="89916-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="89916-122">Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="89916-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="89916-123">En esta fase, debería poder ver el dispositivo de asunto en el estado "pendiente" en la hoja de dispositivos de Azure portal.</span><span class="sxs-lookup"><span data-stu-id="89916-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="89916-124">El registro se completará en el siguiente inicio de sesión de usuario en Windows 10.</span><span class="sxs-lookup"><span data-stu-id="89916-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="89916-125">Si está en VPN y un proceso de inicio de sesión con cierre de sesión finaliza la Conectividad del dominio, puede desencadenar el registro manualmente:</span><span class="sxs-lookup"><span data-stu-id="89916-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="89916-126">Emita un dsregcmd/join localmente en el símbolo del administrador o de forma remota a través de PSExec en su PC.</span><span class="sxs-lookup"><span data-stu-id="89916-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="89916-127">Por ejemplo, PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="89916-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="89916-128">Para obtener más información sobre problemas de combinaciones híbridas, consulte solucionar problemas de [dispositivos](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="89916-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
