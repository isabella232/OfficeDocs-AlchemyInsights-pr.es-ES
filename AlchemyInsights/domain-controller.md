---
title: 'Controlador de dominio '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886901"
---
# <a name="domain-controller"></a><span data-ttu-id="d9c70-102">Controlador de dominio</span><span class="sxs-lookup"><span data-stu-id="d9c70-102">Domain controller</span></span>

<span data-ttu-id="d9c70-103">**No se puede habilitar AAD-DS o la implementación falla**</span><span class="sxs-lookup"><span data-stu-id="d9c70-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="d9c70-104">Para resolver el problema por el que Azure AD Domain Services (AAD-DS) no se habilita o no se implementa correctamente, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="d9c70-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="d9c70-105">Si usa una red virtual ya existente, busque en su NSG reglas que bloquean puertos necesarios para sincronizar con AAD-DS en el portal https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="d9c70-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="d9c70-106">Compruebe si hay una respuesta para el mensaje de error en esta guía de solución de problemas que está disponible en https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="d9c70-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="d9c70-107">Pruebe a implementar Azure AD Domain Services en una nueva red virtual.</span><span class="sxs-lookup"><span data-stu-id="d9c70-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="d9c70-108">Siga la guía de Introducción sobre cómo implementar AAD-DS que está disponible en [Tutorial para crear Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="d9c70-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="d9c70-109">Si tiene problemas con la implementación de Azure AD Domain Services, consulte [Solución de problemas de Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) para resolver errores comunes y obtener ayuda para restaurar el funcionamiento.</span><span class="sxs-lookup"><span data-stu-id="d9c70-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="d9c70-110">**No se puede deshabilitar AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="d9c70-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="d9c70-111">AAD-DS no se puede pausar.</span><span class="sxs-lookup"><span data-stu-id="d9c70-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="d9c70-112">Si quiere dejar de usar el dominio administrado, debe eliminarlo.</span><span class="sxs-lookup"><span data-stu-id="d9c70-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="d9c70-113">Si tiene problemas, para resolver mensajes de error comunes y para conocer los pasos de solución de problemas asociados que le ayudarán a que todo vuelva a funcionar, consulte [Solución de problemas de Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="d9c70-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
