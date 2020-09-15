---
title: Crear un correo electrónico atrapar todo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713003"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="8df9b-102">Crear un correo electrónico atrapar todo</span><span class="sxs-lookup"><span data-stu-id="8df9b-102">Create an email catch all</span></span>

<span data-ttu-id="8df9b-103">No se recomienda el uso de una instrucción Catch.</span><span class="sxs-lookup"><span data-stu-id="8df9b-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="8df9b-104">Es mejor proporcionar un rebote al remitente que permita que los remitentes sepan que no se pudo entregar el mensaje como dirigido para que puedan actuar.</span><span class="sxs-lookup"><span data-stu-id="8df9b-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="8df9b-105">También puede limitar el buzón supervisado para que solo detecte direcciones de correo electrónico válidas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="8df9b-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="8df9b-106">Cualquier buzón de correo de tipo catch recibirá una buena cantidad de correo no deseado y puede, eventualmente, completarse si no está bien supervisado.</span><span class="sxs-lookup"><span data-stu-id="8df9b-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="8df9b-107">(Hay límites de recepción).</span><span class="sxs-lookup"><span data-stu-id="8df9b-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="8df9b-108">Si decide continuar, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="8df9b-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="8df9b-109">Cree un grupo de distribución dinámico & incluya "todos los tipos de destinatarios".</span><span class="sxs-lookup"><span data-stu-id="8df9b-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="8df9b-110">Cree un buzón dedicado para capturar los mensajes de correo electrónico, por ejemplo, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="8df9b-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="8df9b-111">Para el dominio específico, establezca DomainType en "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="8df9b-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="8df9b-112">Si más tarde quita la instrucción Catch, asegúrese de volver a establecer el dominio en autoritativo.</span><span class="sxs-lookup"><span data-stu-id="8df9b-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="8df9b-113">Cree una regla de transporte de flujo de flujo como sigue:</span><span class="sxs-lookup"><span data-stu-id="8df9b-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="8df9b-114">Si el remitente es "fuera de la organización"</span><span class="sxs-lookup"><span data-stu-id="8df9b-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="8df9b-115">Redirigir el mensaje a Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="8df9b-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="8df9b-116">Excepto si el destinatario es miembro de allusers@domain.com (el grupo de distribución contiene todos los miembros)</span><span class="sxs-lookup"><span data-stu-id="8df9b-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="8df9b-117">Asegurarse de que valida que los nuevos buzones se agregan al grupo de distribución dinámico</span><span class="sxs-lookup"><span data-stu-id="8df9b-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
