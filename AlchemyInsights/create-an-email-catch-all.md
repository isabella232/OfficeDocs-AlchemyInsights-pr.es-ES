---
title: Crear un correo electrónico capturar todo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816217"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="35e3e-102">Crear un correo electrónico capturar todo</span><span class="sxs-lookup"><span data-stu-id="35e3e-102">Create an email catch all</span></span>

<span data-ttu-id="35e3e-103">El uso de una captura de todo está muy desaconsejado.</span><span class="sxs-lookup"><span data-stu-id="35e3e-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="35e3e-104">Es mejor proporcionar un rebote al remitente que le permite a los remitentes saber que su mensaje no se pudo entregar como se ha dirigido para que puedan tomar medidas.</span><span class="sxs-lookup"><span data-stu-id="35e3e-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="35e3e-105">También puede limitar el buzón supervisado para que solo pueda capturar direcciones de correo electrónico que antes eran válidas.</span><span class="sxs-lookup"><span data-stu-id="35e3e-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="35e3e-106">Cualquier buzón de correo catch recibirá una gran cantidad de correo no deseado y, finalmente, puede rellenarse si no se supervisa de cerca.</span><span class="sxs-lookup"><span data-stu-id="35e3e-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="35e3e-107">(Hay límites de recepción).</span><span class="sxs-lookup"><span data-stu-id="35e3e-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="35e3e-108">Si decide continuar, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="35e3e-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="35e3e-109">Crear un grupo de distribución dinámico & incluir "Todos los tipos de destinatarios".</span><span class="sxs-lookup"><span data-stu-id="35e3e-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="35e3e-110">Cree un buzón dedicado para capturar correos electrónicos, por ejemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="35e3e-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="35e3e-111">Para el dominio específico, establezca DomainType en "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="35e3e-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="35e3e-112">Si más adelante quita la captura de todo, asegúrese de volver a establecer el dominio en Autoritativo.</span><span class="sxs-lookup"><span data-stu-id="35e3e-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="35e3e-113">Cree una regla de transporte de flujo de correo de la siguiente manera:</span><span class="sxs-lookup"><span data-stu-id="35e3e-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="35e3e-114">Si el remitente es "Fuera de la organización"</span><span class="sxs-lookup"><span data-stu-id="35e3e-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="35e3e-115">Redirigir el mensaje a Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="35e3e-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="35e3e-116">Excepto si el destinatario es miembro de allusers@domain.com (el grupo de distribución contiene todos los miembros)</span><span class="sxs-lookup"><span data-stu-id="35e3e-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="35e3e-117">Asegúrese de validar que los nuevos buzones se agregan al grupo de distribución dinámica</span><span class="sxs-lookup"><span data-stu-id="35e3e-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
