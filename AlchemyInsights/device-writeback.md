---
title: Escritura reescribición de dispositivos
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255174"
---
# <a name="device-writeback"></a><span data-ttu-id="db8e9-102">Escritura reescribición de dispositivos</span><span class="sxs-lookup"><span data-stu-id="db8e9-102">Device Writeback</span></span>

<span data-ttu-id="db8e9-103">La reescribición de dispositivos se usa en los siguientes escenarios:</span><span class="sxs-lookup"><span data-stu-id="db8e9-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="db8e9-104">Habilitar [Windows Hello para empresas mediante la implementación híbrida de certificados de confianza](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="db8e9-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="db8e9-105">Habilitar el acceso condicional basado en dispositivos a aplicaciones protegidas de ADFS (2012 R2 o superior) (confianzas de usuario autenticado)</span><span class="sxs-lookup"><span data-stu-id="db8e9-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="db8e9-106">Se requiere una suscripción a Azure AD Premium para la reescribición de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="db8e9-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="db8e9-107">Esto proporciona seguridad adicional y garantía de que el acceso a las aplicaciones solo se concede a dispositivos de confianza.</span><span class="sxs-lookup"><span data-stu-id="db8e9-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="db8e9-108">Para obtener más información [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) sobre el acceso condicional, vea Administración de riesgos con acceso condicional y configuración del acceso condicional local mediante el registro de [dispositivos de Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="db8e9-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="db8e9-109">Para obtener más información sobre cómo habilitar la escritura reescribición de dispositivos para dispositivos, consulta [Habilitar la escritura reescribición de dispositivos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="db8e9-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
