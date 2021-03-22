---
title: El Acceso condicional con dispositivo unido a dominio me bloquea
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965472"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="746b6-102">El Acceso condicional con dispositivo unido a dominio me bloquea</span><span class="sxs-lookup"><span data-stu-id="746b6-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="746b6-103">**Herramientas altamente recomendadas**</span><span class="sxs-lookup"><span data-stu-id="746b6-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="746b6-104">[Herramienta solucionador de problemas de registro de dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/): la herramienta que ayuda a solucionar los problemas de registro de dispositivos más comunes.</span><span class="sxs-lookup"><span data-stu-id="746b6-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="746b6-105">[Script de conectividad de registro de dispositivos de prueba](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : el script que ayuda a asegurarse de que un dispositivo pueda tener acceso a los puntos de conexión de Registro de dispositivos en la cuenta del sistema.</span><span class="sxs-lookup"><span data-stu-id="746b6-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="746b6-106">[Script de limpieza de dispositivos de Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) : el script que le permite buscar y administrar dispositivos obsoletos en su entorno.</span><span class="sxs-lookup"><span data-stu-id="746b6-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="746b6-107">Aquí tiene algunos motivos habituales por los que el acceso condicional puede fallar en un dispositivo que se haya unido a un dominio (Azure AD híbrido).</span><span class="sxs-lookup"><span data-stu-id="746b6-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="746b6-108">**No hay PRT de Azure AD en el dispositivo**: debe asegurarse de que el dispositivo tenga el token de actualización principal (PRT) de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="746b6-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="746b6-109">Para más información sobre PRT, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="746b6-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="746b6-110">Para comprobar que tiene PRT de Azure AD, puede ejecutar `dsregcmd/status` comando en el dispositivo y comprobar si “AzureAdPrt” es igual a “SÍ”.</span><span class="sxs-lookup"><span data-stu-id="746b6-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="746b6-111">Si “AzureAdPrt” es igual a “NO”, compruebe lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="746b6-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="746b6-112">**Si tiene un entorno federado con AD FS y las redes domésticas de los usuarios no lo pueden alcanzar**: en este caso, asegúrese de que sus puntos de conexión "usernamemixed" sean accesibles desde la extranet.</span><span class="sxs-lookup"><span data-stu-id="746b6-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="746b6-113">Si su AD FS se encuentra detrás de una VPN, asegúrese de que los usuarios se conecten a la VPN y vuelvan a iniciar sesión en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="746b6-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="746b6-114">Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="746b6-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="746b6-115">**Si el TPM del dispositivo es defectuoso y por tanto no puede autenticar el dispositivo**: compruebe "tpm.msc" para ver si el estado del TPM es "Listo".</span><span class="sxs-lookup"><span data-stu-id="746b6-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="746b6-116">Si no es así, ejecute `dsregcmd/leave` y deje que el dispositivo se vuelva a unir a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="746b6-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="746b6-117">A continuación, inténtelo de nuevo.</span><span class="sxs-lookup"><span data-stu-id="746b6-117">Then, try again.</span></span> <span data-ttu-id="746b6-118">Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="746b6-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="746b6-119">**Está usando un proveedor de identidad de terceros que no admite el protocolo WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="746b6-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="746b6-120">Como describimos en nuestros documentos, los dispositivos unidos a Azure AD híbrido no pueden funcionar en este caso.</span><span class="sxs-lookup"><span data-stu-id="746b6-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="746b6-121">Contacte con su proveedor de identidad para obtener soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="746b6-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="746b6-122">**Los usuarios usan el explorador Chrome sin las cuentas de Windows 10** o **extensiones de Office de Chrome no usan automáticamente el PRT en dispositivos unidos a AAD o a AAD híbrido**: esto provoca que cualquier directiva de acceso condicional basado en dispositivos falle, y en dicho caso se muestra el mensaje de error “Dispositivo no registrado”.</span><span class="sxs-lookup"><span data-stu-id="746b6-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="746b6-123">Para usar el explorador Chrome correctamente, debe instalar “Cuentas de Windows 10” o "Extensión de Office para el explorador Chrome de los usuarios" mediante SCCM o Intune.</span><span class="sxs-lookup"><span data-stu-id="746b6-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="746b6-124">Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="746b6-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="746b6-125">Si no es posible instalar la extensión de forma remota, notifique a los usuarios para que instalen manualmente una de las extensiones anteriores para acceder a aplicaciones detrás del acceso condicional basado en dispositivos.</span><span class="sxs-lookup"><span data-stu-id="746b6-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="746b6-126">Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="746b6-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="746b6-127">**El dispositivo estaba unido a Azure AD híbrido correctamente, pero se eliminó o se deshabilitó de manera accidental, ya sea debido a cambios en la sincronización en Azure AD Connect o desde Azure Portal**: si esto sucede, el objeto de dispositivo ya no será reconocido como dispositivo unido de manera completa, aunque los estados "AzureAdJoined" y "PRT" se muestren como válidos en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="746b6-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="746b6-128">Para solucionar este problema, ejecute `dsregcmd/leave` en los dispositivos afectados y deje que se vuelvan a unir a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="746b6-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="746b6-129">Para más información, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="746b6-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="746b6-130">Si sus dispositivos usan Windows 10, actualización 1809, con VPN/Cloud proxy y observa problemas con el estado "AzureAdPrt" o cualquier aplicación con problema de SSO (Outlook no se conecta al buzón de correo pese a tener PRT), asegúrese de tener esta revisión [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) o la actualización acumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para prevenir errores de PRT en esos equipos.</span><span class="sxs-lookup"><span data-stu-id="746b6-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















