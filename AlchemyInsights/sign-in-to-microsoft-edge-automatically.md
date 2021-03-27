---
title: Iniciar sesión en Microsoft Edge automáticamente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398746"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="c412d-102">Iniciar sesión en Microsoft Edge automáticamente</span><span class="sxs-lookup"><span data-stu-id="c412d-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="c412d-103">Microsoft Edge usa la cuenta predeterminada del sistema operativo para iniciar sesión automáticamente en un usuario de acuerdo con la configuración del dispositivo del usuario.</span><span class="sxs-lookup"><span data-stu-id="c412d-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="c412d-104">A continuación se describen los escenarios de cada tipo de configuración de dispositivo y su proceso de inicio de sesión de usuario dependiente:</span><span class="sxs-lookup"><span data-stu-id="c412d-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="c412d-105">**El dispositivo es híbrido/AAD-J:** esta opción está disponible en Windows 10, Windows de nivel inferior y las versiones de servidor correspondientes.</span><span class="sxs-lookup"><span data-stu-id="c412d-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c412d-106">Los usuarios inician sesión automáticamente con sus cuentas de Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="c412d-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="c412d-107">**El dispositivo está unido a un** dominio: esta opción está disponible en Windows 10, Windows de nivel inferior y las versiones de servidor correspondientes.</span><span class="sxs-lookup"><span data-stu-id="c412d-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c412d-108">De forma predeterminada, los usuarios con cuentas de dominio no han iniciado sesión automáticamente; para habilitar el inicio de sesión automático para ellos, use la **directiva ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="c412d-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="c412d-109">Para habilitar el inicio de sesión automático para los usuarios con cuentas de Azure AD, considere la posibilidad de unir híbridos a sus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c412d-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="c412d-110">La cuenta predeterminada del sistema operativo es una cuenta **de Microsoft:** esta opción está disponible en Windows 10 RS3 (versión 1709, compilación 10.0.16299) y versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="c412d-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="c412d-111">Es poco probable que el escenario se produzca en dispositivos empresariales.</span><span class="sxs-lookup"><span data-stu-id="c412d-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="c412d-112">Sin embargo, si la cuenta predeterminada del sistema operativo es una cuenta de Microsoft, Microsoft Edge iniciará sesión automáticamente en el usuario con la cuenta de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c412d-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
