---
title: Dispositivo en estado pendiente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652245"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="7bc8f-102">Dispositivo en estado pendiente</span><span class="sxs-lookup"><span data-stu-id="7bc8f-102">Device in pending state</span></span>

<span data-ttu-id="7bc8f-103">**Requisitos previos**</span><span class="sxs-lookup"><span data-stu-id="7bc8f-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="7bc8f-104">Si está configurando registros de dispositivos por primera vez, asegúrese de que ha revisado la [Introducción a la administración de dispositivos en Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , que le guiarán en la obtención de dispositivos bajo el control de Azure ad.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="7bc8f-105">Si registra los dispositivos directamente en Azure AD y los inscribe en Intune, deberá asegurarse de que ha [configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) y de que el [otorgamiento de licencias](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) se realice primero.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="7bc8f-106">Asegúrese de que tiene autorización para realizar operaciones en Azure AD y AD local.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="7bc8f-107">Solo un administrador global de Azure AD puede administrar la configuración de los registros de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="7bc8f-108">Además, si está configurando los registros automáticos en su Active Directory local, tendrá que ser administrador de Active Directory y AD FS (si procede).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="7bc8f-109">El proceso de registro de Unión híbrida de Azure AD requiere que los dispositivos estén en la red corporativa.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="7bc8f-110">También funciona con VPN, pero hay algunas advertencias.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="7bc8f-111">Hemos oído que los clientes necesitan asistencia para solucionar el proceso de registro de Unión híbrida de Azure AD en circunstancias laborales remotas.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="7bc8f-112">**Entorno de autenticación en la nube (mediante la sincronización de hash de contraseña de Azure AD o la autenticación de paso a través)**</span><span class="sxs-lookup"><span data-stu-id="7bc8f-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="7bc8f-113">Este flujo de registro también se conoce como "sincronización de sincronización".</span><span class="sxs-lookup"><span data-stu-id="7bc8f-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="7bc8f-114">Este es un desglose de lo que sucede durante el proceso de registro:</span><span class="sxs-lookup"><span data-stu-id="7bc8f-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="7bc8f-115">Windows 10 detecta el registro de punto de conexión de servicio (SCP) cuando el usuario inicia sesión en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="7bc8f-116">En primer lugar, el dispositivo intenta recuperar información de inquilinos del SCP del lado cliente en el registro [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="7bc8f-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="7bc8f-117">Para obtener más información, consulte [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="7bc8f-118">Si se produce un error, el dispositivo se comunica con Active Directory local para obtener la información de inquilino de SCP.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="7bc8f-119">Para comprobar el SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="7bc8f-120">Le recomendamos que habilite el SCP en Active Directory y solo use el SCP del lado cliente para la validación inicial.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="7bc8f-121">Windows 10 intenta comunicarse con Azure AD en el contexto del sistema para autenticarse en Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="7bc8f-122">Puede comprobar si el dispositivo puede tener acceso a los recursos de Microsoft en la cuenta del sistema mediante el [script de conectividad de registro de dispositivos de prueba](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="7bc8f-123">Windows 10 genera un certificado autofirmado y lo almacena en el objeto de equipo en Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="7bc8f-124">Esto requiere línea de vista a controlador de dominio.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="7bc8f-125">El objeto de dispositivo que tiene el certificado se sincroniza con Azure AD a través de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="7bc8f-126">El ciclo de sincronización es cada 30 minutos de forma predeterminada, pero depende de la configuración de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="7bc8f-127">Para obtener más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="7bc8f-128">En esta fase, debería poder ver el dispositivo de asunto en el estado "**pendiente**" en la hoja de dispositivos de Azure portal.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="7bc8f-129">El registro se completará en el siguiente inicio de sesión de usuario en Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7bc8f-130">Si está en VPN y cierre de sesión/inicio de sesión finaliza la Conectividad del dominio, puede desencadenar el registro manualmente.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="7bc8f-131">Para ello:</span><span class="sxs-lookup"><span data-stu-id="7bc8f-131">To do that:</span></span>
    >
    > <span data-ttu-id="7bc8f-132">Emita un `dsregcmd /join` mensaje local en el administrador o de forma remota a través de PSExec en su PC.</span><span class="sxs-lookup"><span data-stu-id="7bc8f-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="7bc8f-133">Por ejemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="7bc8f-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="7bc8f-134">Para problemas comunes con el registro de dispositivos de Azure Active Directory, consulte [preguntas más frecuentes sobre dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="7bc8f-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
