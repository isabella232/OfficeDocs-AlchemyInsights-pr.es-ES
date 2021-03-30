---
title: Single-Sign para dispositivos unidos a Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403831"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="e59f8-102">Inicio de sesión único para dispositivos unidos a Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e59f8-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="e59f8-103">Si tiene un entorno de Active Directory (AD) local y desea unir los equipos unidos a un dominio de AD a Azure AD, puede hacerlo mediante la combinación híbrida de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e59f8-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="e59f8-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="e59f8-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="e59f8-105">Configurar dispositivos unidos a Azure AD para dispositivos locales Single-Sign En el uso de Windows Hello para empresas</span><span class="sxs-lookup"><span data-stu-id="e59f8-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="e59f8-106">Problemas del token de actualización **principal (PRT)** Un token de actualización principal (PRT) es un artefacto clave de la autenticación de Azure AD en windows 10, Windows Server 2016 y versiones posteriores, dispositivos iOS y Android.</span><span class="sxs-lookup"><span data-stu-id="e59f8-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="e59f8-107">Se trata de un token web JSON (JWT) especialmente emitido a los agentes de tokens de microsoft para habilitar el inicio de sesión único (SSO) en todas las aplicaciones usadas en esos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e59f8-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="e59f8-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span><span class="sxs-lookup"><span data-stu-id="e59f8-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="e59f8-109">**WamDefaultSet: YES y AzureADPrt: SÍ** Estos campos indican si el usuario se ha autenticado correctamente en Azure AD al iniciar sesión en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e59f8-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="e59f8-110">Si los valores son **NO,** podría deberse a:</span><span class="sxs-lookup"><span data-stu-id="e59f8-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="e59f8-111">Clave de almacenamiento mala en el TPM asociado con el dispositivo al registrarse (comprueba KeySignTest mientras se ejecuta con privilegios elevados).</span><span class="sxs-lookup"><span data-stu-id="e59f8-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="e59f8-112">Identificador de inicio de sesión alternativo</span><span class="sxs-lookup"><span data-stu-id="e59f8-112">Alternate Login ID</span></span>
- <span data-ttu-id="e59f8-113">Proxy HTTP no encontrado</span><span class="sxs-lookup"><span data-stu-id="e59f8-113">HTTP Proxy not found</span></span>

<span data-ttu-id="e59f8-114">Solucionar problemas de dispositivos mediante el comando dsregcmd: [estado de SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="e59f8-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
