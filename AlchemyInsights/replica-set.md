---
title: Conjunto de réplicas
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716279"
---
# <a name="replica-set"></a><span data-ttu-id="72bee-102">Conjunto de réplicas</span><span class="sxs-lookup"><span data-stu-id="72bee-102">Replica set</span></span>

<span data-ttu-id="72bee-103">AADDS también se llama como dominio administrado.</span><span class="sxs-lookup"><span data-stu-id="72bee-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="72bee-104">En realidad, el back-end ejecuta y mantiene dos controladores de dominio.</span><span class="sxs-lookup"><span data-stu-id="72bee-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="72bee-105">Los dos DC incluyen un CONTROLADOR de dominio principal y un CONTROLADOR de dominio de replicación.</span><span class="sxs-lookup"><span data-stu-id="72bee-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="72bee-106">Las copias de seguridad en AADDS (dominio administrado) son un proceso automatizado administrado por la plataforma de Azure.</span><span class="sxs-lookup"><span data-stu-id="72bee-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="72bee-107">En caso de que se produce un problema con el dominio administrado, el soporte técnico de Azure puede ayudarle a restaurar desde la copia de seguridad.</span><span class="sxs-lookup"><span data-stu-id="72bee-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="72bee-108">Cada conjunto de réplicas se crea en una red virtual.</span><span class="sxs-lookup"><span data-stu-id="72bee-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="72bee-109">Cada red virtual debe estar emparejada con todas las demás redes virtuales que hospedan el conjunto de réplicas de un dominio administrado.</span><span class="sxs-lookup"><span data-stu-id="72bee-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="72bee-110">Esta configuración crea una topología de red de malla que admite la replicación de directorios.</span><span class="sxs-lookup"><span data-stu-id="72bee-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="72bee-111">Una red virtual puede admitir varios conjuntos de réplicas, siempre que cada conjunto de réplicas esté en una subred virtual diferente.</span><span class="sxs-lookup"><span data-stu-id="72bee-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="72bee-112">Para obtener más información sobre el conjunto de réplicas, vea [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="72bee-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
