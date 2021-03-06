---
title: Configuración del servicio de aprovisionamiento
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480757"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="ec7b9-102">Configuración del servicio de aprovisionamiento</span><span class="sxs-lookup"><span data-stu-id="ec7b9-102">Configuring the Provision service</span></span>

<span data-ttu-id="ec7b9-103">Para que el aprovisionamiento automatizado de usuarios funcione, Azure AD requiere credenciales válidas que le permitan conectarse a la API de Servicios web de Workday.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="ec7b9-104">Además, el botón Probar conexión de la aplicación aprovisionamiento de usuarios de Workday a AD también valida si puede conectarse al agente de aprovisionamiento de Azure AD Connect asociado al dominio de AD.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="ec7b9-105">Si Azure Portal devuelve un error al guardar las credenciales, siga los pasos recomendados a continuación:</span><span class="sxs-lookup"><span data-stu-id="ec7b9-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="ec7b9-106">Confirme que ha configurado la cuenta de usuario de Workday Integration System tal como se indica en la sección tutorial Configurar usuario del sistema de [integración en Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="ec7b9-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="ec7b9-107">Confirme que el servicio de agente de aprovisionamiento de Azure AD Connect está en funcionamiento en el servidor windows local mediante la Consola de administración de servicios.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="ec7b9-108">También puede comprobar el estado del agente en Azure Portal haciendo clic en el botón Ver agentes locales.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="ec7b9-109">Asegúrese de escribir el valor del campo "Nombre de usuario de workday" con el formato username@workday-tenant-name.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="ec7b9-110">Si falta el nombre de workday-tenant, se produce un error en la autenticación de Workday.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="ec7b9-111">Si va a configurar la integración con el inquilino de implementación de Workday, tenga en cuenta las horas de inactividad programadas del inquilino de Workday.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="ec7b9-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="ec7b9-113">En raras ocasiones, también puede ver este error si la contraseña del usuario del sistema de integración cambió debido a la actualización del inquilino o si la cuenta está en estado bloqueado o expirado.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="ec7b9-114">Compruebe el estado del usuario del sistema de integración con el administrador de Workday.</span><span class="sxs-lookup"><span data-stu-id="ec7b9-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="ec7b9-115">Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="ec7b9-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
