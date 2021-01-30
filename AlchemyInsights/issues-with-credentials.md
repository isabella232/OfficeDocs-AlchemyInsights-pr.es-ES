---
title: Problemas con las credenciales
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052956"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="c8c6e-102">Problemas con las credenciales</span><span class="sxs-lookup"><span data-stu-id="c8c6e-102">Issues with credentials</span></span>

<span data-ttu-id="c8c6e-103">La plataforma de identidad de Microsoft y el flujo de credenciales de cliente de [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describen cómo programar directamente con el flujo de concesión de credenciales de cliente de OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="c8c6e-104">**¿Cómo puedo administrar las credenciales de certificado o contraseña de una aplicación?**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="c8c6e-105">En la CLI de Azure, puedes usar la credencial az [ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, enumerar o restablecer las credenciales de certificado o contraseña de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="c8c6e-106">**¿Cómo restablecen mis usuarios sus contraseñas?**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="c8c6e-107">Los usuarios deben [registrarse para el restablecimiento](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) de contraseña de autoservicio antes de poder restablecer sus contraseñas.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="c8c6e-108">Una vez que un usuario se ha registrado, puede seguir las instrucciones de este artículo para restablecer su contraseña: Restablecer la contraseña del trabajo o [la escuela.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="c8c6e-109">**¿Cómo cambian mis usuarios sus contraseñas?**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="c8c6e-110">Los usuarios pueden seguir los pasos de este artículo para cambiar sus contraseñas: [Cómo cambiar la contraseña.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="c8c6e-111">También pueden administrar [contraseñas de aplicaciones para la verificación en dos pasos.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="c8c6e-112">**Mi usuario recibe un error al cambiar o restablecer su contraseña**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="c8c6e-113">Este vínculo proporcionará información sobre problemas comunes que pueden surgir cuando un usuario intenta restablecer su contraseña: problemas [comunes y sus soluciones](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="c8c6e-114">**Tengo un problema al restablecer la contraseña de un usuario**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="c8c6e-115">Asegúrese de que está autorizado a restablecer contraseñas.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="c8c6e-116">*Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.*</span><span class="sxs-lookup"><span data-stu-id="c8c6e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="c8c6e-117">Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="c8c6e-118">Asegúrese de comprender los requisitos de licencia:</span><span class="sxs-lookup"><span data-stu-id="c8c6e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="c8c6e-119">Debe tener al menos una licencia asignada en su organización:</span><span class="sxs-lookup"><span data-stu-id="c8c6e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="c8c6e-120">**Solo usuarios en la** nube: cualquier SKU de pago de Office 365 (O365) o Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="c8c6e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="c8c6e-121">**Usuarios locales o en** la nube: Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="c8c6e-122">Para obtener más información sobre los requisitos de licencia, consulte Requisitos de licencia para el restablecimiento de contraseña de autoservicio [de Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="c8c6e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="c8c6e-123">Para restablecer la contraseña de un usuario, busque el usuario en Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="c8c6e-124">A continuación, en la hoja de información general para ese usuario, haga clic en el botón "restablecer contraseña".</span><span class="sxs-lookup"><span data-stu-id="c8c6e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="c8c6e-125">**El botón de restablecimiento de contraseña está en gris**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="c8c6e-126">No está autorizado a restablecer las **contraseñas** de este usuario.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="c8c6e-127">*Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.*</span><span class="sxs-lookup"><span data-stu-id="c8c6e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="c8c6e-128">Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="c8c6e-129">**No veo la hoja de restablecimiento de contraseña**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="c8c6e-130">No está autorizado a restablecer contraseñas.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="c8c6e-131">*Solo los administradores globales, de contraseña y de usuario pueden restablecer las contraseñas de usuario.*</span><span class="sxs-lookup"><span data-stu-id="c8c6e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="c8c6e-132">Los administradores globales también pueden restablecer las contraseñas de otros administradores con privilegios.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="c8c6e-133">**No veo la hoja de integración local en el restablecimiento de contraseña**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="c8c6e-134">La hoja de integración local solo aparece en entornos híbridos, lo que significa que usa la escritura de contraseña para manipular las contraseñas de los usuarios locales.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="c8c6e-135">Esta hoja no se ve si:</span><span class="sxs-lookup"><span data-stu-id="c8c6e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="c8c6e-136">No está usando la escritura reescribición de contraseñas</span><span class="sxs-lookup"><span data-stu-id="c8c6e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="c8c6e-137">Hay un problema con la instalación o conectividad de la escritura de contraseña</span><span class="sxs-lookup"><span data-stu-id="c8c6e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="c8c6e-138">Hay un problema con la instalación y conectividad de Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="c8c6e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="c8c6e-139">Para obtener más información sobre los pasos de solución de problemas con la escritura reescribición de contraseñas, vea [Solucionar problemas de](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback) escritura de contraseña</span><span class="sxs-lookup"><span data-stu-id="c8c6e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="c8c6e-140">**No sé cómo restablecer la contraseña de un usuario**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="c8c6e-141">Inicie sesión en Azure Portal como administrador adecuado.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="c8c6e-142">Vaya a la **hoja Usuarios y grupos,** seleccione **Todos los usuarios.**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="c8c6e-143">Seleccione un usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="c8c6e-144">Para el usuario seleccionado, seleccione **Información general** y, a continuación, en la barra de comandos, seleccione **Restablecer contraseña.**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="c8c6e-145">Seleccione el **botón Restablecer contraseña** y siga las instrucciones de la pantalla.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="c8c6e-146">Solo los restablecimientos realizados a través de **Azure Portal** admiten la reescribición de contraseñas.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="c8c6e-147">**Restablecido la contraseña de un usuario local desde el portal de administración de Office 365 o la aplicación móvil de Office 365, pero el usuario aún no puede iniciar sesión**</span><span class="sxs-lookup"><span data-stu-id="c8c6e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="c8c6e-148">La escritura escritura en contraseña no se admite en este portal.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="c8c6e-149">Restablezca la contraseña del usuario de nuevo en Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c8c6e-149">Reset the user's password again in the Azure portal.</span></span>
