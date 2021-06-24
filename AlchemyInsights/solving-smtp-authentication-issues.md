---
title: Habilitar autenticación SMTP y solución de problemas
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077668"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="cbd6d-102">Habilitar autenticación SMTP y solución de problemas</span><span class="sxs-lookup"><span data-stu-id="cbd6d-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="cbd6d-103">Si desea habilitar la autenticación SMTP para un buzón o recibe un error "Cliente no autenticado", "Autenticación incorrecta" o "SmtpClientAuthentication" con el código 5.7.57, 5.7.3 o 5.7.139 al intentar retransmitir correo electrónico mediante la autenticación de un dispositivo o aplicación con Microsoft 365, realice estas tres acciones para resolver el problema:</span><span class="sxs-lookup"><span data-stu-id="cbd6d-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="cbd6d-104">Deshabilite los [Valores predeterminados de seguridad de Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). Para ello, establezca **Habilitar los valores predeterminados de seguridad** en **No**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="cbd6d-105">a.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-105">a.</span></span> <span data-ttu-id="cbd6d-106">Inicie sesión en el Azure Portal como administrador de seguridad, administrador de acceso condicional o administrador global.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="cbd6d-107">b.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-107">b.</span></span> <span data-ttu-id="cbd6d-108">Vaya a Azure Active Directory >  **Propiedades**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="cbd6d-109">c.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-109">c.</span></span> <span data-ttu-id="cbd6d-110">Seleccione **Administrar los valores predeterminados de seguridad**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="cbd6d-111">d.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-111">d.</span></span> <span data-ttu-id="cbd6d-112">Establezca **Habilitar los valores predeterminados de seguridad** en **No**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="cbd6d-113">e.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-113">e.</span></span> <span data-ttu-id="cbd6d-114">Seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-114">Select **Save**.</span></span>

2. <span data-ttu-id="cbd6d-115">Marque [Habilitar el envío de SMTP de cliente](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) en el buzón con licencia.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="cbd6d-116">a.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-116">a.</span></span> <span data-ttu-id="cbd6d-117">En el Centro de administración de Microsoft 365, vaya a **Usuarios activos** y seleccione el usuario.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="cbd6d-118">b.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-118">b.</span></span> <span data-ttu-id="cbd6d-119">Vaya a la pestaña Correo y, en **Aplicaciones de correo electrónico**, seleccione **Administrar aplicaciones de correo electrónico**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="cbd6d-120">d.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-120">d.</span></span> <span data-ttu-id="cbd6d-121">Asegúrese de que **SMTP autenticado** esté activado (habilitado).</span><span class="sxs-lookup"><span data-stu-id="cbd6d-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="cbd6d-122">e.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-122">e.</span></span> <span data-ttu-id="cbd6d-123">Seleccione **Guardar cambios**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="cbd6d-124">Marque [Deshabilitar la autenticación multifactor (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) en el buzón con licencia.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="cbd6d-125">a.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-125">a.</span></span> <span data-ttu-id="cbd6d-126">Vaya al Centro de administración de Microsoft 365 y, en el menú de navegación izquierdo, seleccione **Usuarios** > **Usuarios activos**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="cbd6d-127">b.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-127">b.</span></span> <span data-ttu-id="cbd6d-128">Seleccione **Autenticación multifactor**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="cbd6d-129">c.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-129">c.</span></span> <span data-ttu-id="cbd6d-130">Seleccione el usuario y deshabilite **Autenticación multifactor**.</span><span class="sxs-lookup"><span data-stu-id="cbd6d-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
