---
title: Solucionar problemas de inicio de sesión único para dispositivos unidos a Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898087"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="64282-102">Solucionar problemas de inicio de sesión único para dispositivos unidos a Azure AD</span><span class="sxs-lookup"><span data-stu-id="64282-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="64282-103">Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="64282-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="64282-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="64282-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="64282-105">Para obtener más información, vea [Configure Azure AD joined devices for Single-Sign On](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)on using Windows Hello for Business .</span><span class="sxs-lookup"><span data-stu-id="64282-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="64282-106">**Problemas del token de actualización principal (PRT)**</span><span class="sxs-lookup"><span data-stu-id="64282-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="64282-107">Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en windows 10, Windows Server 2016 y versiones posteriores, dispositivos iOS y Android.</span><span class="sxs-lookup"><span data-stu-id="64282-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="64282-108">Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="64282-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="64282-109">Para obtener más información sobre cómo se emite, usa y protege un PRT en dispositivos Windows 10, consulta ¿Qué es un token de actualización [principal?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="64282-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="64282-110">**WamDefaultSet: YES y AzureADPrt: SÍ**</span><span class="sxs-lookup"><span data-stu-id="64282-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="64282-111">Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64282-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="64282-112">Si los valores **son NO,** podría deberse a:</span><span class="sxs-lookup"><span data-stu-id="64282-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="64282-113">Clave de almacenamiento mal en el TPM asociado con el dispositivo al registrarse (compruebe keySignTest mientras se ejecuta con privilegios elevados)</span><span class="sxs-lookup"><span data-stu-id="64282-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="64282-114">Identificador de inicio de sesión alternativo</span><span class="sxs-lookup"><span data-stu-id="64282-114">Alternate Login ID</span></span>
- <span data-ttu-id="64282-115">Proxy HTTP no encontrado</span><span class="sxs-lookup"><span data-stu-id="64282-115">HTTP Proxy not found</span></span>

<span data-ttu-id="64282-116">Para solucionar problemas de dispositivos mediante el comando dsregcmd, consulte [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="64282-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
