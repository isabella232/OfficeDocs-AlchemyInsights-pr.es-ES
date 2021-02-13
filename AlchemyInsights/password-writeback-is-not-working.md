---
title: La escritura reescribición de contraseñas no funciona
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232785"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="1ef01-102">La escritura por escritura no funciona</span><span class="sxs-lookup"><span data-stu-id="1ef01-102">Password Writeback is not working</span></span>

<span data-ttu-id="1ef01-103">**Tengo problemas para configurar la escritura difisura de contraseñas**</span><span class="sxs-lookup"><span data-stu-id="1ef01-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="1ef01-104">La escritura reescribición de contraseñas es una característica premium.</span><span class="sxs-lookup"><span data-stu-id="1ef01-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="1ef01-105">Asegúrese de que comprende los requisitos de licencia:</span><span class="sxs-lookup"><span data-stu-id="1ef01-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="1ef01-106">Debe tener al menos una licencia asignada en su organización</span><span class="sxs-lookup"><span data-stu-id="1ef01-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="1ef01-107">**Solo usuarios en la** nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="1ef01-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="1ef01-108">**Usuarios locales o** en la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="1ef01-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="1ef01-109">Para obtener más información sobre los requisitos de licencia, consulte [Requisitos de licencias](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) para el restablecimiento de contraseña de autoservicio de Azure AD</span><span class="sxs-lookup"><span data-stu-id="1ef01-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="1ef01-110">Tiene al menos una cuenta de administrador y una cuenta de usuario de prueba con una de las licencias adecuadas.</span><span class="sxs-lookup"><span data-stu-id="1ef01-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="1ef01-111">Debe conectar Azure AD Connect al emulador del controlador de dominio principal para que funcione la escritura reescribición de contraseñas.</span><span class="sxs-lookup"><span data-stu-id="1ef01-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="1ef01-112">Puede configurar Azure AD Connect para usar un controlador  de dominio principal haciendo clic con el botón secundario en las propiedades del conector de sincronización de Active Directory y, a continuación, **seleccionando configurar particiones de directorio.**</span><span class="sxs-lookup"><span data-stu-id="1ef01-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="1ef01-113">Desde allí, busque la sección de configuración **de** conexión del controlador de dominio y active la casilla titulada **solo usar controladores de dominio preferidos.**</span><span class="sxs-lookup"><span data-stu-id="1ef01-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="1ef01-114">Si el DC preferido no es un emulador de PDC, Azure AD Connect seguirá llegando a la PDC para la escritura en contraseña.</span><span class="sxs-lookup"><span data-stu-id="1ef01-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="1ef01-115">El restablecimiento de contraseña se ha configurado y habilitado en el espacio empresarial.</span><span class="sxs-lookup"><span data-stu-id="1ef01-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="1ef01-116">Para obtener más información, vea [Habilitar a los usuarios para restablecer sus contraseñas de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="1ef01-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="1ef01-117">Asegúrese de que la cuenta de administrador que se usa para habilitar la reescribición de contraseñas sea una cuenta de administrador en la nube (creada en Azure AD no en AD local)</span><span class="sxs-lookup"><span data-stu-id="1ef01-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="1ef01-118">Tiene una implementación local de AD de bosque único o de varios bosques que ejecuta Windows Server 2008 R2, Windows Server 2012 o Windows Server 2012 R2 con los Service Pack más recientes instalados</span><span class="sxs-lookup"><span data-stu-id="1ef01-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="1ef01-119">Tiene instalada la herramienta Azure AD Connect y ha preparado su entorno de AD para la sincronización con la nube.</span><span class="sxs-lookup"><span data-stu-id="1ef01-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="1ef01-120">Antes de probar la escritura reescribición de contraseñas, asegúrate de completar primero una importación completa y una sincronización completa de AD y Azure AD en Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1ef01-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="1ef01-121">Para obtener más información, vea cómo realizar una sincronización completa e [importación completa en Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="1ef01-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="1ef01-122">**I'm having a problem with password writeback connectivity**</span><span class="sxs-lookup"><span data-stu-id="1ef01-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="1ef01-123">Descargar y habilitar la última versión de [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="1ef01-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="1ef01-124">Configuración del firewall: la herramienta Azure AD Connect (1.1.443 y posteriores) necesitará acceso **HTTPS** saliente para:</span><span class="sxs-lookup"><span data-stu-id="1ef01-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="1ef01-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1ef01-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="1ef01-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="1ef01-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="1ef01-127">Permitir que las conexiones inactivas persistan durante al menos 2 o 3 minutos</span><span class="sxs-lookup"><span data-stu-id="1ef01-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="1ef01-128">**I'm still having problems with password writeback**</span><span class="sxs-lookup"><span data-stu-id="1ef01-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="1ef01-129">Si sigue teniendo dificultades, intente deshabilitar y volver a habilitar el servicio de escritura difis para contraseñas en la herramienta Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1ef01-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="1ef01-130">Para obtener más información, vea cómo deshabilitar y volver a habilitar la escritura [difi ón de contraseña](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="1ef01-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
