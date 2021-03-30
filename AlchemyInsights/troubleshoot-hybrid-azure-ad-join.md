---
title: Solución de problemas de dispositivos híbridos unidos a Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401924"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="ba55c-102">Solución de problemas de dispositivos híbridos unidos a Azure AD</span><span class="sxs-lookup"><span data-stu-id="ba55c-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="ba55c-103">Se recomienda encarecidamente asegurarse de que un dispositivo puede acceder a los puntos de conexión de registro de dispositivos en la cuenta del sistema mediante el [Script de prueba de conectividad de registro de dispositivos](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="ba55c-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="ba55c-104">Si está configurando los registros de dispositivos por primera vez, asegúrese de revisar la [Introducción a la administración de dispositivos en Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) para obtener información sobre cómo controlar los dispositivos de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ba55c-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="ba55c-105">Si va a registrar dispositivos en Azure AD directamente e inscribirlos en Intune, asegúrese primero de que [ha configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) y que tiene las [licencias adecuadas](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ba55c-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="ba55c-106">Asegúrese de que está autorizado para realizar operaciones en Azure AD y en AD local.</span><span class="sxs-lookup"><span data-stu-id="ba55c-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ba55c-107">Solo un administrador global de Azure AD puede administrar la configuración de registros de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ba55c-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ba55c-108">Además, si está configurando los registros automáticos en su Active Directory local, necesitará ser administrador de Active Directory y AD FS (si procede).</span><span class="sxs-lookup"><span data-stu-id="ba55c-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ba55c-109">Para más información sobre cómo resolver los posibles problemas con la combinación híbrida, vea [Solucionar problemas de combinación híbrida](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) para configurar dispositivos unidos a Azure AD híbrido y administrar dispositivos con Azure AD Portal. Vea [Configurar dispositivos unidos a Azure AD híbrido (dispositivos locales unidos a un dominio)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) y [Administrar dispositivos con Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ba55c-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ba55c-110">Para resolver los problemas comunes con los dispositivos híbridos unidos a Azure Active Directory (AD), consulte las [Preguntas frecuentes sobre los dispositivos híbridos unidos a Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="ba55c-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
