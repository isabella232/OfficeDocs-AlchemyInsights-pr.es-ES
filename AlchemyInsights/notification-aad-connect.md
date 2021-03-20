---
title: Notificación AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898041"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="72e41-102">Notificación AAD Connect</span><span class="sxs-lookup"><span data-stu-id="72e41-102">Notification AAD Connect</span></span>

- <span data-ttu-id="72e41-103">Asegúrese de que está autorizado a realizar la operación.</span><span class="sxs-lookup"><span data-stu-id="72e41-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="72e41-104">Los administradores globales tienen acceso de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="72e41-104">Global Admins have access by default.</span></span> <span data-ttu-id="72e41-105">Además, puede usar el control de acceso [basado en roles para](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegar el permiso de registro al colaborador.</span><span class="sxs-lookup"><span data-stu-id="72e41-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="72e41-106">Asegúrese de que los puntos de conexión necesarios están habilitados y no bloqueados debido al firewall.</span><span class="sxs-lookup"><span data-stu-id="72e41-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="72e41-107">Para obtener más información, vea [requisitos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="72e41-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="72e41-108">El registro puede producir un error debido a que la capa de red somete a la inspección SSL a la comunicación saliente.</span><span class="sxs-lookup"><span data-stu-id="72e41-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="72e41-109">Asegúrese de que ha comprobado la configuración de notificaciones de Azure AD Connect Health y revise la configuración.</span><span class="sxs-lookup"><span data-stu-id="72e41-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="72e41-110">Para comprender cómo configurar las opciones de notificación de las notificaciones de Azure AD Connect Health, consulte esta [guía](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="72e41-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="72e41-111">Para obtener más información sobre el informe de sincronización de AAD Connect Health y cómo descargarlo, vea Informe de sincronización [de nivel de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="72e41-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="72e41-112">Para solucionar problemas de [alertas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) de mantenimiento de AAD Connect siga la guía de solución de problemas de las alertas de actualización de datos de AAD Connect Health y para las preguntas más frecuentes, vea [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="72e41-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
