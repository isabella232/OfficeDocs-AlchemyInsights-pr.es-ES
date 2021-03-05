---
title: Problema con AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453301"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="18d42-102">Problema con AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="18d42-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="18d42-103">Asegúrese de que está autorizado a realizar la operación.</span><span class="sxs-lookup"><span data-stu-id="18d42-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="18d42-104">Los administradores globales tienen acceso de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="18d42-104">Global Admins have access by default.</span></span> <span data-ttu-id="18d42-105">Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.</span><span class="sxs-lookup"><span data-stu-id="18d42-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="18d42-106">Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall.</span><span class="sxs-lookup"><span data-stu-id="18d42-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="18d42-107">Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="18d42-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="18d42-108">El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.</span><span class="sxs-lookup"><span data-stu-id="18d42-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="18d42-109">Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="18d42-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="18d42-110">Revise la configuración.</span><span class="sxs-lookup"><span data-stu-id="18d42-110">Please review your setting.</span></span> <span data-ttu-id="18d42-111">Esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) puede ayudarle a comprender cómo configurar las opciones de notificación para las notificaciones de estado de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="18d42-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="18d42-112">Para obtener más información sobre el informe de sincronización de AAD Connect Health y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="18d42-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="18d42-113">Para solucionar problemas de alertas de estado de AAD Connect, siga la guía de solución de problemas de las alertas de actualización de datos de [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) y para las preguntas más frecuentes, vea Common [AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="18d42-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
