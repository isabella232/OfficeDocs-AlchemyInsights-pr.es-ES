---
title: Configurar el punto de conexión de servicio (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898067"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="d7543-102">Configurar el punto de conexión de servicio (SCP)</span><span class="sxs-lookup"><span data-stu-id="d7543-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="d7543-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="d7543-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="d7543-104">**Motivo**: no se puede leer el objeto SCP y obtener la información del inquilino de Azure AD</span><span class="sxs-lookup"><span data-stu-id="d7543-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="d7543-105">**Resolución**: consulte la sección [Configurar un punto de conexión de servicio](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="d7543-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="d7543-106">**Plan de acción**</span><span class="sxs-lookup"><span data-stu-id="d7543-106">**Action plan**</span></span>

- <span data-ttu-id="d7543-107">Compruebe si el dispositivo ha recibido el GPO para la validación controlada.</span><span class="sxs-lookup"><span data-stu-id="d7543-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="d7543-108">Asegúrese de que el GPO haya creado las claves de registro.</span><span class="sxs-lookup"><span data-stu-id="d7543-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="d7543-109">Asegúrese de tener dos claves creadas con su identificador de directorio y dominio de onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="d7543-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="d7543-110">**Ajustar la configuración del registro del lado cliente para SCP**</span><span class="sxs-lookup"><span data-stu-id="d7543-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="d7543-111">Utilice el siguiente ejemplo para crear un objeto de directiva de grupo (GPO) para implementar una configuración de registro que configure una entrada de SCP en el registro de sus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d7543-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="d7543-112">Abra una consola de administración de directiva de grupo y cree un nuevo GPO en el dominio.</span><span class="sxs-lookup"><span data-stu-id="d7543-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="d7543-113">Proporcione un nombre a su GPO recién creado (por ejemplo, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="d7543-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="d7543-114">Edite el GPO y localice la siguiente ruta: **Configuración del equipo > Preferencias > Configuración de Windows > Registro**.</span><span class="sxs-lookup"><span data-stu-id="d7543-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="d7543-115">Haga clic derecho en **Registro** y seleccione **Nuevo > Elemento de registro**.</span><span class="sxs-lookup"><span data-stu-id="d7543-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="d7543-116">En la pestaña **General**, configure los ajustes siguientes:</span><span class="sxs-lookup"><span data-stu-id="d7543-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="d7543-117">**Acción**: actualizar</span><span class="sxs-lookup"><span data-stu-id="d7543-117">**Action**: Update</span></span>
    
- <span data-ttu-id="d7543-118">**Subárbol**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="d7543-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="d7543-119">**Ruta clave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="d7543-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="d7543-120">**Nombre del valor**: TenantId</span><span class="sxs-lookup"><span data-stu-id="d7543-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="d7543-121">**Tipo de valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="d7543-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="d7543-122">**Datos del valor**: El GUID o Identificador de directorio de la instancia de Azure AD (este valor se puede encontrar en **Azure Portal > Azure Active Directory > Propiedades > Identificador de directorio**)</span><span class="sxs-lookup"><span data-stu-id="d7543-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="d7543-123">Haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="d7543-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="d7543-124">Haga clic derecho en **Registro** y seleccione **Nuevo > Elemento de registro**.</span><span class="sxs-lookup"><span data-stu-id="d7543-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="d7543-125">En la pestaña **General**, configure los ajustes siguientes:</span><span class="sxs-lookup"><span data-stu-id="d7543-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="d7543-126">**Acción**: actualizar</span><span class="sxs-lookup"><span data-stu-id="d7543-126">**Action**: Update</span></span>
    
- <span data-ttu-id="d7543-127">**Subárbol**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="d7543-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="d7543-128">**Ruta clave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="d7543-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="d7543-129">**Nombre del valor**: TenantName</span><span class="sxs-lookup"><span data-stu-id="d7543-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="d7543-130">**Tipo de valor**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="d7543-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="d7543-131">**Datos del valor**: el nombre de dominio verificado si utiliza un entorno federado como AD FS.</span><span class="sxs-lookup"><span data-stu-id="d7543-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="d7543-132">El nombre de dominio verificado o el nombre de dominio onmicrosoft.com (por ejemplo, contoso.onmicrosoft).com si está utilizando un entorno administrado</span><span class="sxs-lookup"><span data-stu-id="d7543-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="d7543-133">Haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="d7543-133">Click **OK**.</span></span>

7. <span data-ttu-id="d7543-134">Cierre el editor del GPO recién creado.</span><span class="sxs-lookup"><span data-stu-id="d7543-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="d7543-135">Vincule el GPO recién creado a la unidad organizativa deseada que contenga equipos unidos a un dominio que pertenezcan a su conjunto de datos de implementación controlado.</span><span class="sxs-lookup"><span data-stu-id="d7543-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="d7543-136">Para obtener más información, consulte [Validación controlada de la Unión a Azure AD híbrido: Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) y [Solución de problemas de dispositivos de Unión a Azure AD híbrido | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="d7543-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









