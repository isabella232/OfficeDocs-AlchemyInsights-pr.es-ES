---
title: Configurar el servicio de dominio
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884619"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="31578-102">No se puede habilitar AAD-DS o la implementación falla</span><span class="sxs-lookup"><span data-stu-id="31578-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="31578-103">Para resolver el problema por el que Azure AD Domain Services (AAD-DS) no se habilita o no se implementa correctamente, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="31578-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="31578-104">Si usa una red virtual ya existente, busque en su NSG reglas que bloquean puertos necesarios para sincronizar con AAD-DS en el portal https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="31578-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="31578-105">Compruebe si hay una respuesta para el mensaje de error en esta guía de solución de problemas que está disponible en https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="31578-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="31578-106">Pruebe a implementar Azure AD Domain Services en una nueva red virtual.</span><span class="sxs-lookup"><span data-stu-id="31578-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="31578-107">Siga la guía de Introducción sobre cómo implementar AAD-DS: [Crear y configurar los Servicios de dominio de AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="31578-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="31578-108">Si tiene problemas con la implementación de Azure AD Domain Services, consulte [Solución de problemas de Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver errores comunes y obtener ayuda para restaurar el funcionamiento.</span><span class="sxs-lookup"><span data-stu-id="31578-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="31578-109">**No se puede deshabilitar AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="31578-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="31578-110">AAD-DS no se puede pausar.</span><span class="sxs-lookup"><span data-stu-id="31578-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="31578-111">Si quiere dejar de usar el dominio administrado, debe eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="31578-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="31578-112">Para eliminar el dominio administrado, vea [Eliminar AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="31578-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



