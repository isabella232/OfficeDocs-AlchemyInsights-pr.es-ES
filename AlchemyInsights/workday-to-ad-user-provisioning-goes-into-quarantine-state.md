---
title: El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430774"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="a4d3a-102">El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena</span><span class="sxs-lookup"><span data-stu-id="a4d3a-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="a4d3a-103">**El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena y no se crean usuarios en AD**</span><span class="sxs-lookup"><span data-stu-id="a4d3a-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="a4d3a-104">El aprovisionamiento de usuarios de Workday a AD pasa al estado de cuarentena y los registros de auditoría muestran eventos de error de exportación con el mensaje **Error: OperationsError-SvcErr: Se produjo un error de operación. No se ha configurado ninguna referencia superior para el servicio de directorio. Por lo tanto, el servicio de directorio no puede emitir referencias a los objetos externos a este bosque**.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="a4d3a-105">Este error suele mostrarse si la unidad organizativa del contenedor de Active Directory no se ha configurado correctamente o si hay problemas con la asignación de expresiones usada para **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="a4d3a-106">Compruebe la unidad organizativa predeterminada para **Nuevos usuarios** de errores tipográficos.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="a4d3a-107">Asegúrese de que la unidad organizativa especificada ya existe en su AD.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="a4d3a-108">Si usa **parentDistinguishedName** en la asignación de atributos, asegúrese de que siempre se evalúa como un contenedor conocido dentro del dominio de AD.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="a4d3a-109">Compruebe el evento Exportar en los registros de auditoría para ver el valor generado.</span><span class="sxs-lookup"><span data-stu-id="a4d3a-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="a4d3a-110">Para obtener más información sobre cómo configurar Workday para el aprovisionamiento automatizado, vea [Tutorial: configurar Workday para el aprovisionamiento automático de usuarios](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="a4d3a-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

