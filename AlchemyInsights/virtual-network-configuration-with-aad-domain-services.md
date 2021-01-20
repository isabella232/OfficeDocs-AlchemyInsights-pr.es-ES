---
title: Configuración de red virtual con Azure AD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884613"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="2297b-102">Configuración de red virtual con Azure AD Domain Services</span><span class="sxs-lookup"><span data-stu-id="2297b-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="2297b-103">Siga los siguientes pasos para realizar la configuración de red virtual con Azure AD Domain Services:</span><span class="sxs-lookup"><span data-stu-id="2297b-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="2297b-104">Compruebe el estado de su dominio en el Azure Portal https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="2297b-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="2297b-105">Compruebe si su NSG contiene reglas que bloqueen los puertos necesarios para la sincronización en Azure Active Directory Domain Services que estén en el portalhttps://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="2297b-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="2297b-106">Asegúrese de que su red virtual esté implementada en la misma región de Azure que su dominio administrado de Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="2297b-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="2297b-107">Asegúrese de que no tiene ningún dominio con el mismo nombre de dominio disponible en la red virtual.</span><span class="sxs-lookup"><span data-stu-id="2297b-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="2297b-108">Para obtener más información sobre consideraciones de diseño de la red virtual de Azure compatibles con Azure AD Domain Services, consulte [Consideraciones sobre la red virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="2297b-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

